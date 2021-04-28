[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.1003149.svg)](https://doi.org/10.5281/zenodo.1003149) [![License: CC BY-SA 4.0](https://img.shields.io/badge/License-CC%20BY--SA%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-sa/4.0/)

# Citation File Format (CFF) website

This repository holds the sources for <https://citation-file-format.github.io/>.


## Build

The site is built with the [Jekyll]() static site generator and the [Minimal Mistakes]() theme.

To build locally, you will have to have [Ruby]() and the Ruby bundler installed, and run the following commands from the root of the repository.

```ruby
bundle install
bundle exec jekyll serve -w
```

This will serve the site on <http://127.0.0.1:4000>, and changes to Markdown sources will be hot-patched.

## Deploy

Changes are automatically deployed when `master` is pushed to via GitHub Pages.
