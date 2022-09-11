# hugo-theme-mako
Mako theme for [Hugo](https://gohugo.io/) built upon [UI-Kit](https://getuikit.com).

## Getting Started

### Installation
If your site is configured for Git already, add this repo to the `themes/` directory as a submodule:

``` bash
git submodule add https://github.com/Eraph/hugo-theme-mako.git themes/mako
```

Otherwise clone it:

``` bash
git clone https://github.com/Eraph/hugo-theme-mako.git themes/mako
```

And set the theme in your site's config file:

``` toml
theme = "mako"
```

### Configuration

Set the following params as you see fit:

``` toml
[params]
  title = "My Site's Name"
  author = "My Name"
  description = "Something About This Site"
  profilePicture = "path/to.image"
  dateFormat = "02/Jan/2006 15:04 MST"
  sections = ["projects"]
  navigation_taxonomies = [ "series", "categories" ]
```

### Navigation Lists
#### Pages and other sections
Pages in the `pages` directory will be shown without a header in navigation. Add a page with:

``` bash
hugo new pages/my-page-name.md
```

Add the front matter parameter `order` to set the order of pages in the list. The order is smallest to largest.

Specify other sections in `config.toml` as an array, e.g.
``` toml
sections = ["projects"]
```

#### Taxonomies
All tags are shown by default at the bottom of the navigation bar. Other taxonomies can be shown above them by specifying them in the `navigation_taxonomies` array in `config.toml`, for example:

``` toml
navigation_taxonomies = [ "series", "categories" ]
```

## License

This theme is released under the [**MIT**](/LICENSE) License.