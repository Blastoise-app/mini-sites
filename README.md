# mini-sites

Collection of small, standalone static pages served via GitHub Pages. Each mini-site is its own folder at the repo root and is reachable at its own URL.

## Live URLs

Base: `https://blastoise-app.github.io/mini-sites/`

| Site | Folder | URL |
| --- | --- | --- |
| Index | `/` | https://blastoise-app.github.io/mini-sites/ |
| Tack Proposal | `tack-proposal/` | https://blastoise-app.github.io/mini-sites/tack-proposal/ |

## Adding a new mini-site

1. Create a new folder at the repo root, e.g. `my-site/`.
2. Add an `index.html` inside it (plus any assets — keep them relative to the folder).
3. Commit and push. GitHub Pages will serve it at `https://blastoise-app.github.io/mini-sites/my-site/`.
4. Share the direct folder URL with whoever needs it.

## Conventions

- One folder per mini-site, lowercase-kebab-case names.
- Each site is self-contained — no shared assets across sites, so they can evolve independently.
- Use relative paths (`./style.css`, `./img/foo.png`) inside a site so it works under the `/mini-sites/<name>/` subpath.
- `.nojekyll` at the root disables Jekyll processing so folders starting with `_` and other edge cases work as-is.

## Enabling GitHub Pages (one-time)

In the repo settings → Pages → Source: **Deploy from a branch**, Branch: **main**, Folder: **/ (root)**.
