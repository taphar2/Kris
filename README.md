# DJ KrisKaps — Birthday Bash Memories Archive

A static, GitHub Pages-ready event memories website.

## Publish with GitHub Pages

1. Create or open the GitHub repository for the website.
2. Upload **all files and folders in this ZIP** to the repository root.
3. Make sure the main HTML file is named `index.html` and sits at the repository root.
4. Commit the changes.
5. In GitHub, open **Settings → Pages**.
6. Under **Build and deployment**, choose **Deploy from a branch**, select your publishing branch (usually `main`) and the `/ (root)` folder, then save.
7. Wait for GitHub Pages to publish, then open the Pages URL on your phone.

## Current contents

- `index.html` — complete website. Existing event artwork and the prepared sponsor logos are embedded in the page, so it can run as a standalone file.
- `assets/logos/` — separate transparent PNG copies of the sponsor logos for future edits.
- `gallery/` — place event photographs here when ready.
- `videos/` — place event video files here when ready.

## Adding event media later

The gallery and video sections currently show animated blurred thumbnail placeholders by design.

In `index.html`, find:

```js
const galleryImages = [];
const videoHighlights = [];
```

Add image paths to `galleryImages`, for example:

```js
const galleryImages = [
  "gallery/photo-01.jpg",
  "gallery/photo-02.jpg"
];
```

Add video paths to `videoHighlights`, for example:

```js
const videoHighlights = [
  "videos/highlight-01.mp4"
];
```

Then upload those media files into the matching folders and commit the changes. The corresponding placeholder will be hidden when media entries are present.

## Notes

- This is a static site; no build step or package installation is required.
- Keep `index.html` at the repository root for the standard GitHub Pages setup.
- Do not rename the media folders unless you also update the paths in `index.html`.
