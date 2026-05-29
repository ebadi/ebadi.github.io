## ebadi.github.io — Hamid Ebadi's Portfolio

## Running the Web Server with Docker

The easiest way to run the site locally is with Docker Compose:

```bash
docker compose up
```

The site will be available at **http://localhost:4000**

The server watches for file changes and rebuilds automatically (`--watch`). LiveReload is available on port 35729.

To stop the server:

```bash
docker compose down
```

To rebuild the gem bundle (e.g. after changing `Gemfile`):

```bash
docker compose run --rm jekyll bundle install
docker compose up
```

---

## Flexible-Jekyll is a simple and clean theme for Jekyll

[Flexible-Jekyll is a simple and clean theme for Jekyll](https://artemsheludko.github.io/flexible-jekyll/)

## Features

- [Google Fonts](https://fonts.google.com/)
- [Font Awesome](http://fontawesome.io/)
- [Disqus](https://disqus.com/)
- [Analytics](https://analytics.google.com/analytics/web/)
- Support Emoji

## Installation:

Fork the ``master`` branch and follow the [Jekyll Installation Documentation](https://jekyllrb.com/docs/installation/).

## License

GNU General Public License v3.0
