# LuzeN website

The main website for LuzeN — a community and a name shared by games,
software and other projects.

The community has roots around 2016. The name appeared around 2017–2018.

## Stack

- Astro — pages, layouts and components
- Tailwind CSS — styling
- TypeScript — type checking
- pnpm — dependency management

## Requirements

- Node.js 22.12.0 or newer
- pnpm in the version specified by `packageManager` in `package.json`

## Local development

Install the dependencies:

```bash
pnpm install --frozen-lockfile
```

Start the development server in the background:

```bash
pnpm astro dev --background
```

Open the local address printed in the terminal.

Manage the server:

```bash
pnpm astro dev status
pnpm astro dev logs
pnpm astro dev stop
```

## Checks and production build

Check types and Astro components:

```bash
pnpm check
```

Generate the production site:

```bash
pnpm build
```

Preview the production build locally:

```bash
pnpm preview
```

The generated site is placed in `dist/`.

## Project structure

- `src/pages/index.astro` — homepage metadata and section order
- `src/layouts/BaseLayout.astro` — shared HTML structure, header and footer
- `src/components/` — page sections and reusable components
- `src/styles/global.css` — theme colors, fonts and global accessibility styles
- `public/` — files served directly, such as the favicon

## Working on the site

1. Make a focused change.
2. Run `pnpm check` and `pnpm build`.
3. Check the result at narrow and wide viewport sizes.
4. Check navigation with the keyboard when changing interactive elements.
5. Commit the completed change.

## Deployment

Deployment configuration and migration from the previous luzen.pl website
are still being prepared.