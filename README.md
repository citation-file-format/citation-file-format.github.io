[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.1003149.svg)](https://doi.org/10.5281/zenodo.1003149) [![License: CC BY-SA 4.0](https://img.shields.io/badge/License-CC%20BY--SA%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-sa/4.0/)

# Citation File Format (CFF) website

This repository holds the sources for <https://citation-file-format.github.io/>.

The site is built with the [Jekyll](https://jekyllrb.com/) static site generator and the [Minimal Mistakes](https://mmistakes.github.io/minimal-mistakes/) theme.

## Develop and build locally

In order for all links in your local clone to point to pages in your locally served version of the site,
you need to temporarily change the value for `url` in the Jekyll config in [`_config.yml`](https://github.com/citation-file-format/citation-file-format.github.io/blob/main/_config.yml#L44) to `url: http://127.0.0.1:4000`. **Do not commit this change.** If you want to commit changes to the config, make sure you change it back to `url: https://citation-file-format.github.io` first!

### Build locally, with `docker`

If you have docker installed, just run

```shell
docker run --rm --volume="$PWD:/srv/jekyll" --env JEKYLL_ENV=development -p 4000:4000 jekyll/jekyll:4.0 jekyll serve
```

then open your browser to [`http://localhost:4000`](http://localhost:4000).

### Build locally, on your own system

```shell
# Make sure Ruby version >2.5 is installed
ruby --version

# Make sure you have the `gem` binary
gem --version

# Install jekyll and bundler dependencies
sudo gem install jekyll:4.2.0 bundler:2.2.24

# install dependencies
# note: https://bundler.io/blog/2019/05/14/solutions-for-cant-find-gem-bundler-with-executable-bundle.html
bundle config set --local path 'vendor/bundle'
bundle install # ignore the CertificateFailureError ?

bundle exec jekyll serve -w
```

This will serve the site on <http://localhost:4000>, and changes to Markdown sources will be hot-patched.

## Deploy

`main` branch is deployed on GitHub Pages.
