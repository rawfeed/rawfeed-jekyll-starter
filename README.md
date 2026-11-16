# rawfeed-jekyll starter

Starter site for [Rawfeed Jekyll 2](https://rawfeed.github.io/rawfeed-jekyll),
using the `rawfeed` Ruby gem and its TUI theme and CLI.

## Local usage

Requirements: Ruby 3.0+, Bundler, Node.js/npm, and ImageMagick for production
image minification.

```sh
npm install
npm run help
npm run serve
npm run build
```

The npm scripts forward to the Rawfeed CLI. Existing script names such as
`npm run jekyll:build`, `npm run create:resume`, and `npm run minify:files` are
kept as aliases. You can also run commands directly with `bundle exec rawfeed`,
for example `bundle exec rawfeed create:draft`. Production build runs Jekyll
and minifies JavaScript, HTML, and images.

## Docker

```sh
docker compose up --build
```

The development server is available at <http://localhost:4000>.

## Content and languages

Edit the interface and page content under `_data/screen/`. Project entries are
in `_data/screen/projects.yml`. The site builds English and Portuguese by
default. To translate a page, create the matching file under `pt/`, set
`lang: pt`, and keep the same permalink. To translate a post, copy it into
`pt/_posts/`, set `lang: pt`, and preserve its `page_id` and permalink. Add new
language codes to `languages` in `_config.yml`, then add matching Markdown and
`_data/screen/locales/<code>.yml` interface data.

See the [Rawfeed documentation](https://rawfeed.github.io/rawfeed-jekyll/) for
installation, configuration, and command details.
