# Valheim Dedicated Server Help
This project is intended to guide new, and experienced players alike, with setting up and maintaining their *vanilla* dedicated Valheim Servers.


## Prerequisites
- **Git** `>=2.2`: https://git-scm.com
- Any Text editor


## Development
Edit your files with the editor of your choosing. To see the changes on the page directly:

Use `docker-compose up`
- Requires: **[Docker](https://docs.docker.com/engine/install)** and **[Docker-Compose](https://docs.docker.com/compose/install)**

Use `bundle exec jekyll serve --source ./docs --config ./docs/_config.yml --force_polling --livereload --incremental`
- Setup: `bundle install`
- Requires: **[Ruby](https://www.ruby-lang.org/en/downloads)** and **[Bundler](https://bundler.io)**

In both cases, you should be able to open [http://localhost:4000](http://localhost:4000) and see your
edits before committing any change!

The pages are in the `./docs` folder, and the Jekyll uses the [Just the Docs](https://github.com/pmarsceill/just-the-docs) theme.


## Useful links
- https://pmarsceill.github.io/just-the-docs
- https://jekyllrb.com/docs