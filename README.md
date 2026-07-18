# Downtown — A Creative Town on 2b2d

A clean, Apple-inspired homepage for the Downtown community — a curated creative town on the 2b2d anarchy server.

## Deploy to GitHub Pages

1. Push this repo to GitHub.
2. Go to **Settings → Pages**.
3. Under "Branch", select `main` / root.
4. Done — your site is live at `https://nikossrcs2.github.io/downtown/`.

## Structure

```
├── index.html           # Main homepage
├── 404.html             # Custom 404 page
├── _config.yml          # GitHub Pages config
├── .github/workflows/
│   └── deploy.yml       # Auto-deploy every 6h via GitHub Actions
├── resources/
│   ├── griefers.json           # Griefer list (loaded dynamically)
│   ├── cluttered_waypoint_for_baritone.png
│   ├── davids_house.png
│   └── lavenders_backrooms.png
└── README.md
```

## Maintain the griefer list

Edit `resources/griefers.json` — the page loads it dynamically at runtime.
No HTML changes needed. The JSON also tracks when the list was last updated.

## Add builds

Drop new screenshots into `resources/` and add a `<figure class="gallery-card">` block in the `#builds` section of `index.html`.

## Page sections

- **About** — what Downtown is
- **Rules** — two simple rules
- **Builds** — screenshot gallery
- **Griefers** — dynamically loaded from `resources/griefers.json`
- **FAQ** — common questions
- **Apply** — how to join
