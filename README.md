# Jarrod Scherer's Personal Website

My personal landing page, built with Astro and hosted on GitHub Pages.

Live site: https://jarrodscherer.au

## Local development

Mainly here as a reference for myself, but useful if anyone else wants to run the site locally.

You need Node.js and npm installed.

After cloning the repository, install the dependencies:

```sh
npm install
```

Start the development server:

```sh
npm run dev
```

Open the local address printed in the terminal. The preview updates
automatically when you save changes.

Press Control+C in the terminal to stop the server.

## Production build

Build the website:

```sh
npm run build
```

The generated website files are written to `dist/`.

Preview that build locally:

```sh
npm run preview
```

If you change the source files, build again to update this preview.

## Deployment

Pushing to the `main` branch triggers the GitHub Actions workflow in
`.github/workflows/deploy.yml`.

The workflow builds the site and publishes it to GitHub Pages.
Local edits and commits do not update the live website until pushed.

## Project structure

- `src/pages/index.astro` — homepage content and styling.
- `public/` — files copied directly into the production build.
- `public/CNAME` — the custom domain used by the website.
- `astro.config.mjs` — Astro configuration.
- `.github/workflows/deploy.yml` — deployment workflow.

## Images

Blog and project images are hosted in the Cloudflare R2 bucket
`blog-images`, using https://images.jarrodscherer.au.

## Future sites

The main website will remain a personal hub.

Future plans include:

- `warhammer.jarrodscherer.au` — Warhammer hobby blog.
- `projects.jarrodscherer.au` — programming project portfolio.

These sites are not deployed yet. Each is intended to have its own
repository, Astro project, and GitHub Pages deployment.