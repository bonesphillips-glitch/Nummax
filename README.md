# Nummax

Next.js App Router starter with TypeScript, Tailwind CSS 4, ESLint, and npm.

Requires Node.js 20.9 or newer. Dependencies are pinned in `package-lock.json`.

## Install

```sh
npm ci
```

In the cloud environment, use a writable npm cache:

```sh
npm ci --cache /tmp/nummax-npm
```

## Develop

```sh
npm run dev -- --hostname 0.0.0.0 --port 3000
```

The application entry point is `src/app/page.tsx`; the root layout and global styles are next to it. The `@/*` import alias maps to `src/*`. System fonts avoid build-time Google Fonts downloads.

## Validate and run production

```sh
npm run lint
npm run build
npm run start -- --hostname 0.0.0.0 --port 3001
```

Development and production root pages were checked for HTTP 200 and rendered starter content; the production stylesheet was checked for generated Tailwind utility rules. The production build also validates TypeScript.

The earlier Vite concept was preserved outside this repository at `/workspace/backups/nummax-vite-before-next.tar.gz` before initialization. This project is the fresh Next.js starter, not a migration of that design.
