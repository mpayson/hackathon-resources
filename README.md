# Hackathon Resources

> Esri hackathon quick links

_Also find Esri and OS projects on [Github](https://github.com/esri)!_

## Contents

* [Activate Account and Credits](#activate-account-and-credits)
* [Get Started](#get-started)
* [Workflows](#workflows)
* [Hackable Data](#hackable-data)
* [Analytics](#analytics)
* [Libraries](#libraries)
* [Examples](#examples)

## Activate Account and Credits

1. Sign-up for a free developer account at <http://developers.arcgis.com>
2. Sign in to your account
3. Click your name at the top right, click “Redeem Voucher”, then enter `BITCAMP` for 1000 credits

## Get Started

* Overview: [What you can do](https://developers.arcgis.com/features/) || [Core concepts](https://developers.arcgis.com/documentation/) || [Quick start tutorials](https://developers.arcgis.com/labs/) || [Developers Website](https://developers.arcgis.com/)
* Languages: [JavaScript](https://developers.arcgis.com/javascript/) || [Python](https://developers.arcgis.com/python/) || [iOS](https://developers.arcgis.com/ios/latest/) || [Android](https://developers.arcgis.com/android/latest/) || [Node](https://github.com/esri/arcgis-rest-js) || [REST](https://developers.arcgis.com/rest/) || [Other](https://developers.arcgis.com/documentation/)
* Other: [Create proxy](https://developers.arcgis.com/documentation/core-concepts/security-and-authentication/working-with-proxies/) (avoid auth--it's a hackathon!)

## Workflows

***Note**: The [DevLabs](https://developers.arcgis.com/labs/) are the best place to start, [JS](https://developers.arcgis.com/labs/browse/?topic=any&product=JavaScript) || [Python](https://developers.arcgis.com/labs/browse/?topic=any&product=Python) || [iOS](https://developers.arcgis.com/labs/browse/?topic=any&product=iOS) || [Android](https://developers.arcgis.com/labs/browse/?topic=any&product=Android) || [REST](https://developers.arcgis.com/labs/browse/?topic=any&product=REST-API) || [All](https://developers.arcgis.com/labs/browse/?)

### Data Management

***Note**: ArcGIS can host your data then you can access it via our APIs so you don't have to worry about a backend! We refer to data as [layers](https://developers.arcgis.com/documentation/core-concepts/layers/). The links below are for Feature Layers, a common layer type that represents a **table** with point, line, and polygon [geometries](https://developers.arcgis.com/documentation/core-concepts/features-and-geometries/).

* Create new table: [With empty schema](https://developers.arcgis.com/labs/arcgisonline/create-a-new-dataset/) || [From file](https://developers.arcgis.com/labs/arcgisonline/import-data/)
* Upload & host csvs: [Python](https://github.com/mpayson/partner-python-tools/blob/master/bulk_ops/csv_upload.ipynb)
* Edit data in hosted services: [Python](https://github.com/mpayson/partner-python-tools/blob/master/bulk_ops/append_data.ipynb) || [ArcGIS Online Viewer](http://doc.arcgis.com/en/arcgis-online/share-maps/manage-hosted-feature-layers.htm#ESRI_SECTION1_E2F5EF6240F246EBA5D238968B63BF97)
* Bulk geocode csv: [Python](https://github.com/mpayson/partner-python-tools/blob/master/bulk_ops/csv_geocode.ipynb) || [Node](https://github.com/Esri/arcgis-rest-js/tree/master/demos/batch-geocoder-node)

### Design

* [Create 2d web map](https://developers.arcgis.com/labs/arcgisonline/create-a-web-map/): 2D portable abstraction of data and styles
* [Create 3d web scene](https://developers.arcgis.com/labs/arcgisonline/create-a-web-scene/): 3D portable abstraction of data and styles

### Develop

* Add 2d Feature (vector) Layer: [JS](/samples/2dLayer.html) || [iOS](https://developers.arcgis.com/labs/ios/create-a-2d-map-with-a-layer/) || [Android](https://developers.arcgis.com/labs/android/create-a-2d-map-with-a-layer/)
* Add 3d Layer: [JS](/samples/3dLayer.html) || [iOS](https://developers.arcgis.com/ios/latest/swift/sample-code/scene-layer-url-.htm) || [Android](https://developers.arcgis.com/android/latest/sample-code/scene-layer.htm)
* Apply Layer Edits: [JS](/samples/ApplyEdit.html) || [iOS](https://developers.arcgis.com/ios/latest/swift/guide/edit-features.htm) || [Android](https://developers.arcgis.com/android/latest/guide/edit-features.htm#ESRI_SECTION1_2A4C0222216A448C9CBAFCD0F75A21F6)
* Route: [JS](/samples/Route.html) || [iOS](https://developers.arcgis.com/ios/latest/swift/guide/find-a-route.htm) || [Android](https://developers.arcgis.com/labs/android/display-a-route/)

## Hackable Data

* *[About](http://www.arcgis.com/features/maps/index.html)*
* Open Data Portals: [ArcGIS Open Data](http://hub.arcgis.com/pages/open-data) || [ArcGIS Living Atlas](https://livingatlas.arcgis.com/en/) || [Los Angeles Hub](http://geohub.lacity.org/)
* Common categories: [Imagery](https://livingatlas.arcgis.com/en/browse/#s=0&q=landsat&md=imagery:11111) || [Disaster](http://hub.arcgis.com/datasets?q=Disaster) || [Weather](https://livingatlas.arcgis.com/en/browse/#s=0&q=weather) || [Crime](http://hub.arcgis.com/datasets?q=Crime) || [Sustainability](hub.arcgis.com/datasets?q=Sustainable)
* 3D Buildings ([explore](https://www.arcgis.com/home/webscene/viewer.html?webscene=08409d3e2d8543ca81217a88f428a502)): [New York City](https://tiles.arcgis.com/tiles/V6ZHFr6zdgNZuVG0/arcgis/rest/services/NYCatt/SceneServer) || [Berlin](https://tiles.arcgis.com/tiles/P3ePLMYs2RVChkJx/arcgis/rest/services/Buildings_Berlin/SceneServer) || [Philadelphia](http://scenesampleserverdev.arcgis.com/arcgis/rest/services/Hosted/Buildings_Philadelphia/SceneServer) || [Valencia](https://services1.arcgis.com/YFraetVkEAF1lMag/arcgis/rest/services/Valencia_3D_v2_local/SceneServer)
* [Fetch Demographic Data](https://developers.arcgis.com/features/demographics/)

## Analytics

* Imagery Analytics with Python: [Image processing](https://developers.arcgis.com/python/guide/using-imagery-layers/) || [Feature extraction](https://developers.arcgis.com/python/sample-notebooks/counting-features-in-satellite-images-using-scikit-image/)
* [Trace Downstream](https://developers.arcgis.com/rest/elevation/api-reference/trace-downstream.htm)
* [Evaluate Watersheds](https://developers.arcgis.com/rest/elevation/api-reference/watershed.htm)

## Libraries

* [Koop](https://github.com/koopjs/koop): Translate, query, & integrate any geospatial API
* [Teraformer](https://github.com/esri/Terraformer): Convert data between WKT, ArcGIS JSON, and GeoJSON

## Examples

* Artificial Intelligence Talks: [Traffic Cams & Self Organizing Maps](https://youtu.be/Cm_oAaQVWZ8?t=5m14s) || [Utah Accident Prediction](https://youtu.be/aKq50YM8a8w?t=3m11s)
* [Explore Indoors](https://mpayson.github.io/partner-pocs/indoor-reality/index.html)
* [LA Visitor Demographics](https://mpayson.github.io/partner-pocs/safegraph/index.html)
* [Explore buildings in NYC](https://esri.github.io/Manhattan-skyscraper-explorer/)
* [San Francisco Crime](https://coolmaps.esri.com/#4)
* [Urban planning with the City of Philadelphia](https://www.arcgis.com/apps/CEWebViewer/viewer.html?3dWebScene=86f88285788a4c53bd3d5dde6b315dfe)
