# yifanzhou.com

Source for Yifan Zhou's personal website, served by GitHub Pages at [yifanzhou.com](https://yifanzhou.com). Built from the [Academic Pages](https://github.com/academicpages/academicpages.github.io) Jekyll template.

## Where things live

- `_pages/about.md`: homepage (bio, work experience, education)
- `_pages/publications.html`: selected publications list (thumbnails go in `images/`)
- `_config.yml`: name, bio, sidebar links (Google Scholar, LinkedIn, email)
- `_data/navigation.yml`: header menu
- `files/Yifan_Zhou_CV.pdf`: CV linked from the header and homepage. Replace this file to update the CV.

## Running locally

With [Docker](https://www.docker.com/):

```bash
docker build -t jekyll-site .
docker run -p 4000:4000 --rm -v $(pwd):/usr/src/app jekyll-site
```

Or with Ruby 3.x and Bundler installed:

```bash
bundle install
bundle exec jekyll serve -l -H localhost
```

The site is then served at http://localhost:4000 and rebuilds on file changes. Changes to `_config.yml` require restarting the server.
