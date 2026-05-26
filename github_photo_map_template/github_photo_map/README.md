# GitHub Project Photo Map

This package is designed for GitHub Pages.

## Folder structure

```text
project-photo-map/
  index.html
  photo-json-generator.html
  data/
    photos.json
  photos/
    your-project-photos.jpg
```

## Workflow

1. Open `photo-json-generator.html` locally.
2. Drag/drop your geotagged project photos.
3. Download `photos.json`.
4. Put the original photos into `/photos`.
5. Put `photos.json` into `/data`.
6. Commit and push to GitHub.
7. Enable GitHub Pages for the repository.

## Notes

- Do not rename photos after generating the JSON unless you also update the `image` paths in `photos.json`.
- If local testing fails by double-clicking `index.html`, run a local server from the folder:

```bash
python -m http.server 8000
```

Then open:

```text
http://localhost:8000
```

- The aerial map uses free Esri imagery by default. For sharper premium satellite imagery, add a Mapbox token into `index.html`.
