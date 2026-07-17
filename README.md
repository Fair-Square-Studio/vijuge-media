# vijuge-media

Static media host for **Vijuge** game assets, served via GitHub Pages:

```
https://netdrill.github.io/vijuge-media/media/<hash>.webp
```

- Files under `media/` are content-addressed (`<hash16>.webp`) and **immutable, additive-only** — published files are never modified or deleted, since shipped clients may still reference them.
- All images derive from **Wikimedia Commons** under PD / CC0 / CC BY / CC BY-SA licenses. Per-image attribution lives in [`CREDITS.json`](CREDITS.json) and is surfaced in-app.
- This repo is **synced automatically** from the vijuge content pipeline (`scripts/sync-media-repo.sh` in the main repo) — do not edit by hand.
- This is the beta-phase media host; production launch moves to a bucket/CDN behind the same `NEXT_PUBLIC_MEDIA_URL` seam.
