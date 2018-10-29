# react-turf-cutter
React Component to plot and divide spatial data with Leaflet by drawing polygons with Leaflet.Snap

## API

### Cutter Props

| name     | description    | type     | default      |
|----------|----------------|----------|--------------|
| points | List of points to separate | Array | [] |
| centerOnAverage | Whether or not map centers on average of points | bool | true |
| center | Used when `centerOnAverage` is false | Co-ordinates object | false |

## Usage

TODO add `React.render` example, or whole Component. Use [this tool](https://babeljs.io/repl#?babili=false&browsers=&build=&builtIns=false&spec=false&loose=false&code_lz=Q&debug=false&forceAllTransforms=false&shippedProposals=false&circleciRepo=&evaluate=false&fileSize=false&timeTravel=false&sourceType=module&lineWrap=true&presets=es2015%2Creact%2Cstage-2&prettier=false&targets=&version=6.26.0&envVersion=).

```jsx
<TurfCutter
  points={[]}
  callback={function() {}}
  />
```
