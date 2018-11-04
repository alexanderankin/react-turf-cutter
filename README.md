# react-turf-cutter
React Component to plot and divide spatial data with Leaflet by drawing polygons with Leaflet.Snap

## API

### TurfCutter Props

| name     | description    | type     | default      |
|----------|----------------|----------|--------------|
| points | List of points to separate | Array | `[]` |
| pointsId | `points` must be an array of objects with a unique value for the this key | string | `'id'` |
| centerOnAverage | Whether or not map centers on average of points | bool | `true` |
| center | Used when `centerOnAverage` is false | Co-ordinates object | `false` |
| callback | Called with `(err, results)` when results submitted | function | `function () {}` |

Required properties of `point` objects:

1. `'id'` or `pointsId`: unique identifier
1. `location`: String address, or Co-ordinates object (`{ lat: Number, lon: Number }`)


## Usage

TODO add `React.render` example, or whole Component. Use [this tool](https://babeljs.io/repl#?babili=false&browsers=&build=&builtIns=false&spec=false&loose=false&code_lz=Q&debug=false&forceAllTransforms=false&shippedProposals=false&circleciRepo=&evaluate=false&fileSize=false&timeTravel=false&sourceType=module&lineWrap=true&presets=es2015%2Creact%2Cstage-2&prettier=false&targets=&version=6.26.0&envVersion=).

```jsx
<TurfCutter
  points={[
    { id: 1, location: '1600 Forbes Ave, Pittsburgh PA, 15219' },
    { id: 2, location: '1710 Forbes Ave, Pittsburgh PA, 15219' },
    { id: 3, location: '1840 Forbes Ave, Pittsburgh PA, 15219' },
    { id: 4, location: '1850 Forbes Ave, Pittsburgh PA, 15219' }
  ]}
  callback={function(e, r) { alert(JSON.stringify(r, null, 2)); }}
  />
```
