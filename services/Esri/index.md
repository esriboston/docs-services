---

copyright:

  years: 2016

lastupdated: "2017-2-9"

---

{:new_window: target="_blank"}
{:shortdesc: .shortdesc}
{:screen:.screen}
{:codeblock:.codeblock}
{:pre: .pre}

# Getting started with ArcGIS for developers
{: #gettingstarted}

ArcGIS for developers enables you to create and manage apps that include mapping, visualization, analysis, and more. Build web and mobile applications on Bluemix. Start with a basemap, then add your data, and interact using [ArcGIS API for JavaScript](https://developers.arcgis.com/javascript/).

To get started with ArcGIS APIs on Bluemix:

1. Sign up for a free ArcGIS Developer subscription, [sign up for one here](https://developers.arcgis.com/sign-up/){:new_window}.
2. Reference the [ArcGIS API for JavaScript](https://developers.arcgis.com/javascript/) and load the neccessary modules.{:new_window}.
3. Create the map and select one of our many basemaps.
    ![](http://www.arcgis.com/features/img/maps/maps-banner.jpg)

4. Define the view. In the example below it is using a 2D map view, but the API also supports a 3D map view.{:new_window}.

 ```html
  <!DOCTYPE html>
  <html>
  <head>
    <meta charset="utf-8">
    <meta name="viewport" content="initial-scale=1,maximum-scale=1,user-scalable=no">
    <title>Getting Started App</title>

    <link rel="stylesheet" href="https://js.arcgis.com/4.2/esri/css/main.css">

    <style>
      html, body, #viewDiv {
        padding: 0;
        margin: 0;
        height: 100%;
      }
    </style>

    <script src="https://js.arcgis.com/4.2/"></script>

    <script>
      require([
        "esri/Map",
        "esri/views/MapView",
        "dojo/domReady!"
      ], function(Map, MapView) {

        var map = new Map({
          basemap: "dark-gray-vector"
        });

        var view = new MapView({
          container: "viewDiv",
          map: map,
          center: [-122.68, 45.52],
          zoom: 10
        });

      });
    </script>
  </head>
  <body>
    <div id="viewDiv"></div>
  </body>
  </html>
  ```
5. Now that you have a map, go beyond basemaps and imagery and explore maps and data about people and businesses, transportation, and much more with your [ArcGIS developers subscription](https://developers.arcgis.com/content-and-services/).  

	{: pre}

# Related Links
{: #rellinks}

## ArcGIS API for JavaScript
{: #sdk}

* [ArcGIS API for JavaScript](https://developers.arcgis.com/javascript/){:new_window}

## API Reference
{: #api}

* [ArcGIS API for JavaScript](https://developers.arcgis.com/javascript/latest/api-reference/index.html){:new_window}

## Build Native Apps
{: #runtimes}

* [ArcGIS Runtime SDKs](https://developers.arcgis.com/arcgis-runtime/){:new_window}

## Samples
{: #general}

* [ArcGIS API for JavaScript Samples](https://developers.arcgis.com/javascript/latest/sample-code/index.html){:new_window}
* [ArcGIS Runtime SDK for iOS](https://developers.arcgis.com/ios/latest/swift/sample-code/sample-code.htm){:new_window}
* [ArcGIS Runtime SDK for Android](https://developers.arcgis.com/android/latest/sample-code/sample-code.htm){:new_window}
