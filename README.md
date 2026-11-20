# MyLauncher Library

Public library for MyLauncher: themes + wallpapers.

- `index.json` lists everything the app shows.
- `themes/*.json` theme files, `wallpapers/` full images (1080x2400), `thumbs/` small previews.

## Add your own wallpaper
1. Put the image in `wallpapers/` (and optionally a small copy in `thumbs/`).
2. Add an entry to `wallpapers[]` in `index.json`:
   `{"id":"my1","name":"My","name_ar":"خاصتي","file":"wallpapers/my1.jpg","thumb":"thumbs/my1.jpg","category":"mine"}`
   (if `thumb` is missing the app uses `file`).
3. Commit and push. The app picks it up on next open.

## Add a theme
Copy any file in `themes/`, edit colors (`#AARRGGBB`), add an entry to `themes[]` in `index.json`.
