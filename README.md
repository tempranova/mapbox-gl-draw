# mapbox-gl-draw.js

Adds support for drawing and editing features on [mapbox-gl.js](https://www.mapbox.com/mapbox-gl-js/) maps.

[![Circle CI](https://circleci.com/gh/mapbox/mapbox-gl-draw/tree/master.svg?style=svg)](https://circleci.com/gh/mapbox/gl-draw/tree/master)

### Installing

```
npm install mapbox-gl-js
```

Require or include `mapbox-gl-draw` after you `mapbox-gl`.

Also include [mapbox-gl-draw.css](https://github.com/mapbox/mapbox-gl-draw/blob/dev-pages/dist/mapbox-gl-draw.css)

```html
<link href="mapbox-gl-draw.css" rel="stylesheet" />
```

### Usage

```js
mapboxgl.accessToken = 'YOUR_ACCESS_TOKEN';

var map = new mapboxgl.Map({
  container: 'map',
  style: 'mapbox://styles/mapbox/streets-v8',
  center: [40, -74.50],
  zoom: 9
});

var Draw = mapboxgl.Draw();

map.addControl(Draw)
```

### See [API.md](https://github.com/mapbox/mapbox-gl-draw/blob/master/API.md) for complete reference.

### Developing

Install dependencies, build the source files and crank up a server via:

```
git clone git@github.com:mapbox/mapbox-gl-draw.git
npm install
npm start & open http://localhost:9966/debug
```

### Testing

```
npm run test
```
