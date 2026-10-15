# web3D

A browser-based 3D scene builder for creating printable STL designs from simple 2D and 3D elements.

This project is a single-page web app that lets you arrange images, text, and basic geometric forms on a virtual print bed, then export the combined result as an STL file for 3D printing.

Test it now: https://papabibo.github.io/web3D/

## Features

- Import SVG, PNG, and JPG assets
- Convert raster images into printable contours via thresholding and simplification
- Add text with configurable font, size, spacing, and extrusion height
- Add basic forms such as cubes, spheres, cylinders, and torus objects
- Position, rotate, duplicate, mirror, align, and distribute selected objects
- Create holes and boolean subtraction operations
- Add a base plate and manage print-bed dimensions
- Save and reload scene layouts as JSON
- Measure distances with a ruler tool
- Export the composed scene to STL

## Project purpose

`web3D` is designed for makers who want to build custom printable parts quickly in the browser without requiring a full CAD toolchain. It is especially useful for:

- creating embossed text and signage
- converting simple graphics into reliefs
- composing multiple elements into one printable object
- prototyping small custom 3D-printable artifacts

## How it works

1. Open the app in a browser.
2. Upload an image, SVG, or text input.
3. Adjust the target size, extrusion height, and contour settings.
4. Add the element to the scene.
5. Arrange items on the print bed.
6. Export the final composition as an STL file.

## Run locally

Because this project relies on browser modules and CDN imports, the easiest way to run it is to serve the repository locally.

### Option 1: Python

```bash
cd web3D
python3 -m http.server 8000
```

Then open:

```text
http://localhost:8000
```

### Option 2: Any static web server

You can also serve the folder with `vite`, `npx serve`, or any similar static web server.

## Files

- `index.html` — main application and UI
- `README.md` — project overview and usage guide
- `LICENSE` — project license

## Notes

- The app is primarily a frontend/static web application; there is no build step required.
- Some interface labels are in French, but the workflow is straightforward and centered around the scene editor.
- STL export is intended for 3D printing and fabrication workflows.

## License

This project is licensed under the terms included in the `LICENSE` file.

## Contributions

Pull requests and improvements are welcome. If you want to extend the app with new shapes, better SVG handling, or more export options, this repo is a good starting point.
