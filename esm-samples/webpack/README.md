# ArcGIS API for JavaScript with webpack

This repo demonstrates how to use the [`@arcgis/core`](https://www.npmjs.com/package/@arcgis/core) esm modules with webpack.

This repo also uses the [`@arcgis/webpack-plugin@next`](https://www.npmjs.com/package/@arcgis/webpack-plugin) webpack plugin to copy assets and help to minimize your deployed application size. You can read the updated `@arcgis/webpack-plugin` documentation [here](https://github.com/Esri/arcgis-webpack-plugin/tree/update-for-esm). The plugin assists with the copying of the API's assets.

Be sure to set [`config.assetsPath`](https://developers.arcgis.com/javascript/latest/api-reference/esri-config.html#assetsPath) so that the assets are correctly resolved, for example:

```js
import esriConfig from '@arcgis/core/config.js';

esriConfig.assetsPath = './assets'; 
```