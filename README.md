# motor-speed-controller-gui

Single-page web GUI for monitoring and analyzing motor RPM data from an embedded IoT motor speed controller. Renders a live chart with Chart.js and bundles into a single inlined HTML file via webpack.

## Features

- Live RPM graph with configurable point count and zoom in/out
- Data analysing view for stepping through captured data
- Messages framed with `REF-` / `FILE-` headers and `-WEB-END` footer
- Webpack build inlines CSS and JS into one HTML file

## Layout

```
src/
  index.html    markup and controls
  index.js      chart logic and message handling
  style.css     styles
webpack.config.js
package.json
```

## Build

```bash
npm install
npm run build
```

Output is written to `dist/`.
