# Personal Website

This repository contains the source for [burakguenhan.com](https://burakguenhan.com/),
built with Hugo, Wowchemy, and blogdown-style content.

## Local Development

Requirements:

- Hugo Extended `0.101.0`

Useful commands:

```bash
hugo server
```

Starts a local development server with live reload.

```bash
hugo
```

Builds the site into `public/`.

## Deployment

The site is deployed with Netlify using the settings in
[`netlify.toml`](netlify.toml).

## Repository Notes

- Source content lives under `content/`.
- Generated output goes to `public/`.
- Hugo resource caches go to `resources/`.
- Blog posts may include both source `.Rmarkdown` files and generated
  `.markdown` output.
