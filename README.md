# Portless-Docusaurus breakage repro

This is a minimal repro showing that [Portless](https://portless.sh/) does not work out-of-the-box with [Docusaurus](https://docusaurus.io/).

```bash
npm install
npm run dev
```

The Docusaurus site will be available at `localhost:PORT`, but `docusaurus.localhost:1355` does not work.

The Docusaurus default README follows.

---

# Website

This website is built using [Docusaurus](https://docusaurus.io/), a modern static website generator.

## Installation

```bash
yarn
```

## Local Development

```bash
yarn start
```

This command starts a local development server and opens up a browser window. Most changes are reflected live without having to restart the server.

## Build

```bash
yarn build
```

This command generates static content into the `build` directory and can be served using any static contents hosting service.

## Deployment

Using SSH:

```bash
USE_SSH=true yarn deploy
```

Not using SSH:

```bash
GIT_USER=<Your GitHub username> yarn deploy
```

If you are using GitHub pages for hosting, this command is a convenient way to build the website and push to the `gh-pages` branch.
