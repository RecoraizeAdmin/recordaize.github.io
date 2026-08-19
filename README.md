# recordaize.github.io — Image / Asset CDN

Static asset hosting via GitHub Pages. Any file committed to this repo is served at:

```
https://recordaize.github.io/<path-to-file>
```

## Folder structure

```
apps/
  recordaize/
    assets/
      images/
        logos/     ← logo images
        icons/     ← icon images
        banners/   ← banner / hero images
```

## How to add an image

1. Drop the file into the matching folder, e.g. `apps/recordaize/assets/images/logos/raize-full6.png`
2. Commit and push to `main`.
3. Access it at:

```
https://recordaize.github.io/apps/recordaize/assets/images/logos/raize-full6.png
```

## Adding more apps

Replicate the pattern for any new app, e.g. `apps/<app-name>/assets/images/...`.

## Notes

- `.nojekyll` is present so GitHub Pages serves every file (including ones in `_`-prefixed folders) as-is, with no Jekyll processing.
- Allow ~1 minute after pushing for a new/updated file to go live.
- GitHub Pages must be enabled: **Settings → Pages → Source: `main` branch, `/ (root)`**.
