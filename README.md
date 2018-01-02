# Sapling

A simple [Hugo](https://gohugo.io) theme for creating websites of hierarchical content.

Sapling contains builtin templates that put a breadcrumb navigation trail at the top of each page, and a contents listing at the bottom of each section/list page.

Sapling is small, with no JS, very little CSS and just the essential HTML templates. I recommend forking this theme and modifying it for your own purposes rather than just overriding parts of it.

## Installation

If you are new to Hugo you can get started by following the [quick start guide](https://gohugo.io/getting-started/quick-start/).

Once you're set up, you need to get the contents of this repo into a `yoursite/themes/sapling` directory and then add the line `theme = "sapling"` to your `config.toml` file.

Check out the example site included with the theme for some sensible default settings.

## Example Site

If you just want to view a sample site without setting up an existing hugo site, clone the repo then run `hugo serve` in the `example` directory:

```bash
$ git clone https://github.com/kvurd/sapling
$ cd sapling/example
$ hugo serve
```

Then fire up a web browser and point it at `http://localhost:1313`.

## Notes 
### URL Configuration

Sapling works with a variety of URL configurations, specified in your site config file.

- Full absolute URLs. Set baseURL to the full URL of your site. For baseURL = “https://example.com/“ links will render as https://example.com/blog/second/.
- URLs relative to server root. Set baseURL to “/“ (or the root of your site on the server).
- Full relative URLs. Set relativeURLs = true.
- Full relative URLs browsable from your local file system without a web server. Set relativeURLs = true and uglyURLs = true. Also add uglyURLs = true to your params - there's some template logic that depends on this to properly link back to the home page.
