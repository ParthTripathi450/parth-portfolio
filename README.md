# parth-portfolio

Personal site — dark hero with a WebGL Rubik's cube, glass project cards and live
LeetCode stats. Plain static HTML: no build step, no framework, no bundler.

## Structure

    index.html        the portfolio
    images/           project screenshots
    favicon.svg       cube mark
    flow-field.html   experiment: converging flow field (canvas 2D)
    resend-cube.html  experiment: Resend-style hero cube

## Notes

- The cube is Three.js (r128, from cdnjs). Every texture is generated at runtime
  onto a canvas, so there are no image assets for it.
- Tech icons are inlined as base64 data URIs — no icon CDN at runtime.
- LeetCode stats come from a public API with CORS enabled; a fallback in
  `index.html` renders if it is unreachable.
- The nav robot is a Spline scene loaded from prod.spline.design.

Open `index.html` directly, or serve the folder with any static server.
