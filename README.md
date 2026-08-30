# GT:Classic website

Source code and build config for the [GT:Classic](https://github.com/GTClassic) website.

## Developing

Install dependencies and start a dev server:

```sh
pnpm install
pnpm dev
```

Open the printed URL (defaults to http://localhost:5173). The server auto-reloads on changes.

## Building

Create a production build, output to the `build/` directory:

```sh
pnpm build
```

Preview the production build locally:

```sh
pnpm preview
```

Run the type-checker and linter before pushing:

```sh
pnpm check
pnpm lint
```

## Deploying to Cloudflare Pages

The site uses `@sveltejs/adapter-static`, so the whole site is pre-rendered into static files at
build time and can be hosted anywhere a static file server works.

### Manage Pages / dashboard

1. Push this repository to a Git host (e.g. GitHub or GitLab).
2. In Cloudflare Pages, create a new project and connect the repository.
3. Set the following build settings:
   - **Framework preset:** SvelteKit
   - **Build command:** `pnpm build`
   - **Build output directory:** `build`
   - **Root directory:** `/` (leave as the default, or set it if your repo lives in a subfolder)
   - **Node.js version:** 18 or newer
4. Cloudflare Pages will automatically deploy on every push to the connected branch.

### Wrangler CLI

```sh
pnpm add -D wrangler

# deploy directly
npx wrangler pages deploy build --project-name <your-project-name>

# or preview locally
npx wrangler pages dev build
```

To use the CLI with the same project every time, add a `wrangler.toml`:

```toml
name = "<your-project-name>"
compatibility_date = "2024-01-01"

[pages]
  build_command = "pnpm build"
  output_dir = "build"
```

Then build and deploy with `npx wrangler pages deploy`.
