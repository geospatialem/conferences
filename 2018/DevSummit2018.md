# Esri Developer Summit 2018 (Palm Springs, Cali.)

<img src="https://user-images.githubusercontent.com/5023024/37805637-78080310-2e09-11e8-8d33-6f174f2f9aa3.gif" alt="Esri logo" width="75" height="25"> [Esri Developer Summit](http://www.nacis.org) is designed to show you how to build cutting-edge apps using advanced mapping technology from Esri. At DevSummit you will be the first to see new tools for geo-enabling your apps to get pro tips from the developers who made them.  

## Tuesday, March 6, 2018
* [Plenary](#plenary-multiple-esri-staff), Multiple Esri staff    
* [Navigating Your Way Through the ArcGIS API for JavaScript Sessions]((#navigating-your-way-through-the-arcgis-api-for-javaScript-sessions-multiple-esri-staff), Multiple Esri staff    
* [Using ArcGIS REST JS and REST APIs](#using-arcgis-rest-js-and-rest-apis-john-gravois-dave-bouwman-and-tom-wayson), [John Gravois](https://twitter.comjgravois), [Dave Bouwman](https://twitter.com/dbouwman) and [Tom Wayson](https://twitter.com/tomwayson) [[Slides](https://tomwayson.github.io/devsummit-2018/arcgis-rest-js.html), [Repo](https://github.com/Esri/arcgis-rest-js), [Website](https://esri.github.io/arcgis-rest-js)]  
* [Tracking User Engagement for Feedback and Quality with Telemtry.js](#tracking-user-engagement-for-feedback-and-quality-with-telemtry-js-markham-shofner-and-daniel-fenton), [Markham Shofner](https://twitter.com/markhamshofner) and [Daniel Fenton](https://twitter.com/dmfenton) [[NPM package](https://www.npmjs.com/package/@esri/telemetry)]
* [Develop with Confidence: CT/CI/CD](#develop-with-confidence-ct-ci-cd-idi-eradiri), [Idi Eradiri](https://github.com/joppa27)    
* [ArcGIS API for JS Programming Patterns and API Fundamentals](#arcgis-api-for-js-programming-patterns-and-api-fundamentals-matt-driscoll-and-rene-rubalcava), [Matt Driscoll](https://twitter.com/driskull) and [Renè Rubalcava](https://twitter.com/odoenet) [[Slides](https://odoe.github.io/presentations/2018-PS-DevSummit/jsapi4-patterns-fundamentals)]

# Wednesday, March 7, 2018
# Thursday, March 8, 2018  
# Friday, March 9, 2018


## Tuesday, March 6, 2018

### Plenary - Multiple Esri Staff  
1. Zillow housing data from Living Atlas [[Video](https://www.youtube.com/watch?v=RP3rk_fcc3Y&list=PLaPDDLTCmy4aE-073hhwZQplvJ8MmKZCe&index=5), [GitHub](http://ycabon.github.io/2018-devsummit-plenary)]
  * Also can be downloaded from [Zillow's research site](https://www.zillow.com/research/data/).  
2. Mobile 3D [[Video](https://www.youtube.com/watch?v=XqbBY3iXyaU&index=8&list=PLaPDDLTCmy4aE-073hhwZQplvJ8MmKZCe)]
3. New Widgets [[Video](https://www.youtube.com/watch?v=EEuhqJQHWH8&index=9&list=PLaPDDLTCmy4aE-073hhwZQplvJ8MmKZCe)]   
  * Coordinate conversion (Projection operations in browser)
  * LayerList (has build-in legend)
  * Legend (card style)
4. Widget functionality [[Video](https://www.youtube.com/watch?v=0Kmmha5sBZU&index=10&list=PLaPDDLTCmy4aE-073hhwZQplvJ8MmKZCe)]
  * Keyboard accessible and `:focus`  
  * Popup (expand/collapse)
  * Search widget (incl. geolocator)
5. Typescript [[Resource](https://developers.arcgis.com/javascript/latest/guide/typescript-setup/index.html)]
6. Python Notebooks: ArcGIS API for Python [[Video](https://www.youtube.com/watch?v=nppRAj-OZ6k&list=PLaPDDLTCmy4aE-073hhwZQplvJ8MmKZCe&index=15)]  
7. ArcGIS for Developers Updates [[Video](https://www.youtube.com/watch?v=aTYSTwkYv2E&list=PLaPDDLTCmy4aE-073hhwZQplvJ8MmKZCe&index=17)]
  * [ArcGIS DevLabs](https://developers.arcgis.com/labs)    
  * Example apps
8. ArcObjects 10.6 will be continued to be supported [[Video](https://www.youtube.com/watch?v=6CqAF-OPZ0E&index=18&list=PLaPDDLTCmy4aE-073hhwZQplvJ8MmKZCe)]
  * Resources on GitHub  
9. ArcGIS Pro [[Video](https://www.youtube.com/watch?v=qrp46oVBiEY&list=PLaPDDLTCmy4aE-073hhwZQplvJ8MmKZCe&index=20)]
  * Automate/extend with Python or .NET (Visual Studio)
  * Debugging for Python
  * Encrypted Python tools (Source code hidden when shipped)
10. Offline maps (working with Maps) [[Video](https://www.youtube.com/watch?v=3q-JoOkW4Vo&list=PLaPDDLTCmy4aE-073hhwZQplvJ8MmKZCe&index=23)]  

### Navigating Your Way Through the ArcGIS API for JavaScript Sessions - Multiple Esri Staff [[Blog post](http://esriurl.com/webdev2018devsummit)]  
1. What's new *
2. 2D Visualization *
3. Tips & Tricks Debugging *  
4. Building Widgets (4.x) *  
5. App Design & CSS Styling *  
6. Customize API for JS Widgets   
7. Program Patterns & API Fundamentals *  
8. Angular 5  
9. Typescript  
10. Customize Layers
11. Optimizing JavaScript for Performance
12. JS Apps for Enterprise: Build for Production *
13. JS Apps for Enterprise: Test more, work less *
14. Using Frameworks with ArcGIS API for JS
15. Geometry Engine (client side) *
16. Mobile
17. Integrate with Portal/AGOL
18. JS: The Road Ahead *  

### Using ArcGIS REST JS and REST APIs - John Gravois, Dave Bouwman, and Tom Wayson  
* Written in Typescript  
* Small and lightweight  

#### Goals
* Analogous to the Python API
* Node.js & modern browsers  
* A la carte  
* Framework agnostic  
* "Shave down sharp edges"  

#### End Product  
* Open-ended, put in parameters as-needed  
* Currently only supporting text (images coming soon)  
* In Cedar, items and groups, Hub JS API, Esri Leaflet, [dev.arcgis.com](https://developers.arcgis.com)

#### Demos
See https://github.com/Esri/arcgis-rest-js/tree/master/demos      
* [batch-geocoder-node](https://github.com/Esri/arcgis-rest-js/tree/master/demos/batch-geocoder-node)  
* [tomwayson/hub-errors](https://github.com/tomwayson/hub-events) *(To be posted in the Esri repo.)*  
* [feature-service-browser](https://github.com/Esri/arcgis-rest-js/tree/master/demos/feature-service-browser)


### Tracking User Engagement for Feedback and Quality with Telemtry.js, Markham Shofner and Daniel Fenton     
#### Installation  
Source code coming soon to GitHub  
```
npm esri/telemetry
```

#### Principles  
Anonymize user base, since it goes back to Google Analytics.  
* Referrals  
* Location  
* Devices  
* **User Explorer**  

#### Planning Ahead  
* Users goals  
* Event categories  
* Common actions  
* Custom dimensions

##### Tracking
1. Page views  
2. Events - Events people are doing  
3. Errors - Must be built in  
4. Workflow  

#### User Explorer  
* Add segment
* **Search on site, can be added to Google's search terms.**  

#### Google Search Console  
* Organic searches  
* **Google Analytics Query Explorer**
  * Raw data out of Google Analytics  


### Develop with Confidence: CT/CI/CD, Idi Eradiri    
#### Continuous Integration (CI)  
* Feature branch up-to-date with mainline branch.
* e.g. A GitHub update between local and repo up (up-to-date)

#### Continuous Delivery (CD)  
* `master` change → Deployed to production  
* Automated tests help with deployment   

#### Continuous Deployment  
* **Agile/Dev Ops goal**  
* Every change that meets criteria is pushed to production.

#### Goal  
Better software to users/customers with stable with a consistent development pipeline.  

#### Tools
Jenkins and Slack are integrated together.   
1. GitHub
2. Jenkins (Docker, Travis, Bamboo, ...) - Deployment pipelines, release  
3. Slack - Helps with situational awareness
  * Jenkins also sent to GitHub

#### Pipeline  
Build → Test * → Deploy

#### Test *  
* DBUnit
* JUnit
* Jasmine

**Browser**:  
* Chrome  
* Edge  
* Firefox  
* Safari  

#### Perfect Software  
* No such thing  
* Automate build and deployment pipeline to focus on features. Helps fix bugs faster.  

#### Lessons Learned    
* Automate as much as possible (e.g. system down for maintenance, system up again).
* Patience - give team time to adapt to a change in the process.  


### ArcGIS API for JS Programming Patterns and API Fundamentals, Matt Driscoll and Rene Rubalcava  

#### Fundamentals
* Map and view   
* Basemap, Ground, and Operational Layers  
* LayerViews  
* Widgets and UI  
* ArcGIS Platform  

#### Programming Patterns
* Interactivity with Input Manager  
* Working with Accessor  
* Promises  
* Loadable  

#### Map and View  
* `Map` has information about the layers (what the :earth_americas: is composed of).
* `Mapview` and `SceneView` displays each layer on the screen (a window on that :earth_americas:)  

![Map and View](https://user-images.githubusercontent.com/5023024/37868921-c9e21a76-2f7c-11e8-8945-ae5b5edab9c7.png)  


**Code**:  
```javascript  
/* Getting started in 2D */

//1. Need a `map` with data
//2. Need a `MapView` with a container
const map = new Map({
  basemap: "topo"
});

const view = new MapView({
  map: map,
  container: "viewDiv"
});
```  

```javascript  
/* Getting started in 3D */

//1. Need a `map` with data
//2. Need a `SceneView` with a container
const map = new Map({
  basemap: "topo"
});

const view = new SceneView({
  map: map,
  container: "viewDiv"
});
```  

#### Basemap, Ground, and Operational Layers  
* Separated into three groups:  [1] `basemap`, [2] `ground`, and [3] operational `layers`.  
* `basemap` and `ground` gives context to the operational `layers`.
* `basemap` and `ground` can be set by well-known ids or item id (recommended for production).  
* `Map.layers` contains `Layer` objects with the operational data the user interacts with.  
* A layer can only be in one place.  
* There are layers in multiple places:  
  * Pro: Easy to swap a basemap with another.  
  * Pro: Easy to reproduce a tree structure of the data.  
  * Pro: Easy to manager a group of layer.  
  * Con: More places to look for changes.  
* Layers can be searched using `Map.allLayers`, and contains the layers from **every** collection.  

**Basemap & Ground Well-known ids example**:
```javascript  
const map = new Map({
  /*
  Basemap options: streets, satellite, hybrid, terrain, topo, gray, dark-gray, oceans, national-geographic, osm, dark-gray-vector, gray-vector, streets-vector, topo-vector, streets-night-vector, streets-relief-vector, streets-navigation-vector
  */
  basemap: "streets",
  ground: "world-elevation"
})
```

**Specifying example:**:  
```javascript  
const map = new Map({
  basemap: {
    baseLayers: [ //Layers drawn at the bottom
      new TileLayer({
        url: baselayerUrl
      })
    ],
    referenceLayers: [ //Layers drawn on top
      new TileLayer({
        url: refUrl
      })
    ],
  },
  ground: {
    layers: [
      new ElevationLayer({
        url: elevationUrl
      })
    ]
  }
})
```  

**Item ID example**:  
```javascript  
require([
  "esri/Map",
  "esri/views/MapView",
  "esri/layers/TileLayer",
  "esri/layers/VectorTileLayer"
], function(
  EsriMap,
  MapView,
  TileLayer,
  VectorTileLayer) {

  const map = new Map({
    basemap: {
      baseLayers: [
        new TileLayer({
          url: "https://services.arcgisonline.com/arcgis/rest/services/Elevation/World_Hillshade/MapServer"
        }),
        new VectorTileLayer({
          portalItem: {
            id: "86d5ed4b6dc741de9dad5f0fbe09ae95"
          }
        })
      ]
    }
  });

  const view = new MapView({
    container: "viewDiv",
    map: map,
    center: [-116.5, 33.80],
    scale: 50000
  });

});
```
**Get all of the map layers example**:
```javascript
const layer = map.allLayers.find(layer => {
  return layer.title === "what I'm looking for";
});
```

#### Layers  

**TileLayer**:  
* Displays square images stitched together.
* Fast display becauses tiles are cached.
* URL points to a map service.  

```javascript
const transportationLyr = new TileLayer({
  url: "https://server.arcgisonline.com/ArcGIS/rest/services/Reference/World_Transportation/MapServer",
  id: "streets",
  visible: false
});
```

**WebTileLayer [[API Sample](https://developers.arcgis.com/javascript/latest/sample-code/layers-webtile-3d/index.html), [OSM Sample](https://developers.arcgis.com/javascript/latest/sample-code/layers-osm-3d/index.html)]**:  
* For use with machine serving map tiles.  
* Define the: `level`, `column`, and `row`.  

```javascript  
const tiledLayer = new WebTileLayer({
  urlTemplate: "http://{subDomain}.tile.stamen.com/toner/{level}/{col}/{row}.png",
  subDomains: ["a", "b", "c", "d"],
  copyright: "Map tiles by <a href=\"http://stamen.com/\">Stamen Design</a>, " +
    "under <a href=\"http://creativecommons.org/licenses/by/3.0\">CC BY 3.0</a>. " +
    "Data by <a href=\"http://openstreetmap.org/\">OpenStreetMap</a>, " +
    "under <a href=\"http://creativecommons.org/licenses/by-sa/3.0\">CC BY SA</a>."
});
```

**GraphicsLayer [[2D sample](https://developers.arcgis.com/javascript/latest/sample-code/intro-graphics/index.html), [3D sample](https://developers.arcgis.com/javascript/latest/sample-code/graphics-basic-3d/index.html)]**:  
* Simplest layer to work with.  
* Symbolizes `Graphic` object on the view.  
* A `graphic` requires a geometry and a symbol (no renderer, so must have symbology attached).  
* Can attach attribute and a popup template.  

```javascript  
const graphicsLayer = new GraphicsLayer({
  graphics: [graphic1, graphic2, graphic3]
});
//Add a single graphic
graphicsLayer.add(graphic4);
//Add an array of graphics
graphicsLayer.addMany([graphic5, graphic6, graphic7]);
```  

```javascript  
/* Create a graphic */
const graphic = new Graphic({
  attributes: {
    id: 1,
    city: "Los Angeles"
  },
  geometry: { type: "point", x: xValue, y: yValue },
  symbol: {
    type: "simple-marker",
    style: 'circle',
    color: 'red',
    size: 10,
    outline: {
      color: "rgba(255, 255, 255, 0.5)"
      width: 4
    }
  },
  popupTemplate: {
    title: "My Awesome Graphic!",
    content: "{*}" // display all fields
  }
});
// add it to graphicsLayer
graphicsLayer.add(graphic);
```

**FeatureLayer**:  
* Displays features (`geometry` and `attributes`).  
* Features are fetched from a service, or local collection.  
* Feature geometry is the same for the entire layer.  
* Cannot be symbolized individually (`Feature.renderer`).  

```javascript  
// Create via URL
const featureLayer = new FeatureLayer({
  url: "http://services6.arcgis.com/m3L8QUZ93HeaQzKv/arcgis/rest/services/BeerAndBurgerJoints/FeatureServer/0"
});

// Create via a Portal item
const featureLayer = new FeatureLayer({
  portalItem: {
    id: "b126510e440744169943fd8ccc9b0c4e"
  }
});
```  

**FeatureLayer (WebGL)**:  
* To display > 180,000 features.  
* Hosted feature services.
* Includes selection location  

```html
<script>  
var dojoConfig = {
  has: {
    "esri-featurelayer-webgl": 1
  }
};
</script>
```

**MapImageLayer [[CodePen example](https://codepen.io/odoe/pen/QQPwGw)]**:  
* Previously called Dynamic Map Service.    
* Displays layers and sublayers from Map Services.  
* Map Service can export map image given a bounding box.  
* Simplified API for dynamic layer infos
(sublayers).  

```javascript  
const layer = new MapImageLayer({
  url: "https://sampleserver6.arcgisonline.com/arcgis/rest/services/USA/MapServer",
  sublayers: [
  {
    id: 0,
    visible: true
  },
  {
    id: 1,
    visible: true
  },
  {
    id: 2,
    visible: true,
    definitionExpression: "pop2000 > 1000000"
  },
  {
    id: 3,
    visible: false
  }]
});
```

**SceneLayer [[CodePen example](https://codepen.io/odoe/pen/GQLgxL)]**    
#### LayerViews [[CodePen example](https://codepen.io/odoe/pen/NymGbB)]  
![Layerview](https://user-images.githubusercontent.com/5023024/37869573-b72dd50e-2f87-11e8-895e-1fe6bb9def84.png)  
* LayerViews renders the layers on the screen.  
* [LayerView](https://developers.arcgis.com/javascript/latest/api-reference/esri-views-layers-LayerView.html) has limited API so far.  
* Give info about layer rendering.  
* Give access to data displayed on the screen (Features, Elevation data).
* Access with `view.whenLayerView()` (cleaner method) or `view.allLayerViews`.  
* `FeatureLayer` and `LayerViews` can be queried.
  *  Query features on the service: `featureLayer.queryFeatures()`.
  * Query features on the client: `featureLayerView.queryFeatures()`


#### Widgets and UI
* New design and experience (accessibility, UX, extensibility)
* New architecture (Views and ViewModels)
* Styling (Sass, [Styling Guide](https://developers.arcgis.com/javascript/latest/guide/styling/index.html), [CSS Themes](https://odoe.github.io/presentations/2018-PS-DevSummit/jsapi4-patterns-fundamentals/demos/ui/themes.html), [GitHub JSAPI Resources SASS](https://github.com/Esri/jsapi-resources/blob/master/4.x/bower/dojo/SASS.md))
* Logic of the widget separated from the representation.    
* Provide APIs to support view.  
* [ZoomViewModel](https://developers.arcgis.com/javascript/latest/api-reference/esri-widgets-Zoom-ZoomViewModel.html)

**Widget views [[Demo](https://odoe.github.io/presentations/2018-PS-DevSummit/jsapi4-patterns-fundamentals/demos/widgets/viewModel-use.html), [Widget Development Doc](https://developers.arcgis.com/javascript/latest/guide/custom-widget/index.html), [Custom Widget Tutorial](https://developers.arcgis.com/javascript/latest/sample-code/widgets-custom-widget/index.html)]**:  
* Extends [`esri/widgets/Widget`](https://developers.arcgis.com/javascript/latest/api-reference/esri-widgets-Widget.html)  
* Rely on `ViewModel`  
* Focus on UI
* Views' source code available in the [SDK](https://developers.arcgis.com/javascript/latest/api-reference/esri-widgets-Zoom.html).  
* View's can be rewritten in any framework using ViewModels.  

#### UI [[UI Guide](https://developers.arcgis.com/javascript/latest/guide/view-ui/index.html), [Demo](https://odoe.github.io/presentations/2018-PS-DevSummit/jsapi4-patterns-fundamentals/demos/ui/padding.html)]  
* Managed overlay to place widget over the view.  
* Padding  
  * UI.padding defined spacing for widgets/UI.
  * View.padding defined spacing for center, extent, etc (work off subsection of the full view).
* [Well known widgets](https://developers.arcgis.com/javascript/latest/api-reference/esri-views-ui-DefaultUI.html#components) can be added/removed from the view.

[Demo](https://odoe.github.io/presentations/2018-PS-DevSummit/jsapi4-patterns-fundamentals/demos/ui/manual.html):  

```javascript
/* API to add widgets or any DOM element to the 4 corners of the view */
const view = new MapView({
  //...
});

const legend = new Legend({
  //...
});

view.ui.add(legend, "top-left");
```

#### Popups [[Documentation](https://developers.arcgis.com/javascript/latest/api-reference/esri-PopupTemplate.html#content)]  
* Responsive  
* First entry point to detailed data  

```javascript  
/* Basic popup */
const featureLayer = new FeatureLayer({
  url: "https://sampleserver6.arcgisonline.com/arcgis/rest/services/Census/MapServer/3",
  outFields: ["*"],
  popupTemplate: {
    title: "Name: {STATE_NAME}",
    content: "{*}"
  }
});
```

**Content example**:  
```javascript  
content: [
  {
    type: "fields",
    fieldInfos: [
      {
        fieldName: "POP2000",
        visible: true,
        label: "Population for year 2000",
        format: {
          places: 0,
          digitSeparator: true
        }
      },
      ...  
    ]
  }
]
```  

**Format dates**:  

```javascript  
{
  fieldName: "FAKEDATE",
  visible: true,
  label: "Fake Date Field",
  format: {
    dateFormat: "short-date"
  }
}
```  

**Field and Aliases**:  
```javascript  
const featureLayer = new FeatureLayer({
  url: "https://sampleserver6.arcgisonline.com/arcgis/rest/services/Census/MapServer/2",
  outFields: ["*"],
  popupTemplate: {
    title: "Name: {STATE_NAME}",
    content: `
      <section>
        <h4>{STATE_ABBR}</h4>
        <hr />
        <ul>
          <li>Year 2000 Pop: {POP2000}</li>
          <li>Year 2007 Pop: {POP2007}</li>
          <li>Total Households: {HOUSEHOLDS}</li>
        </ul>
      </section>
    `
  }
});
```  

**Media Infos**:  
```javascript  
{
  type: "media",
  mediaInfos: [
    {
      title: "<b>Population</b>",
      type: "column-chart",
      caption: "",
      value: {
        theme: "BlueDusk",
        fields: [ "POP2000", "POP2007" ]
      }
    }
  ]
}
```  

**Charts**:  
```javascript  
{
  type: "media",
  mediaInfos: [
    {
      title: "<b>Population</b>",
      type: "column-chart",
      caption: "",
      value: {
        theme: "BlueDusk",
        fields: [ "POP2000", "POP2007" ]
      }
    }
  ]
}
```  

**Custom actions [[Demo](https://odoe.github.io/presentations/2018-PS-DevSummit/jsapi4-patterns-fundamentals/demos/widgets/popup-actions.html)]**:  
```javascript  
// PopupTemplate
{
  title: '{Name}',
  content: '{*}',
  actions: [{
      id: 'alcohol-details',
      className: 'esri-icon-description',
      title: 'Events'
  }]
}
```   
**Dock Options [[Documentation](https://developers.arcgis.com/javascript/latest/api-reference/esri-widgets-Popup.html#dockOptions), [Demo](https://odoe.github.io/presentations/2018-PS-DevSummit/jsapi4-patterns-fundamentals/demos/widgets/popup-dockOptions.html)]**:  
```javascript  
view.popup.set("dockOptions", {
  breakpoint: false,
  buttonEnabled: false,
  position: "bottom-center"
});
```   

**Arcade [[Documentation](https://developers.arcgis.com/arcade/), [Demo](https://odoe.github.io/presentations/2018-PS-DevSummit/jsapi4-patterns-fundamentals/demos/widgets/popup-arcade.html)]**:  
```javascript  
popupTemplate: new PopupTemplate({
  title: "Arcade Example",
  content: "{expression/total} total items.",
  expressionInfos: [{
    "name": "total",
    "title": "Total Items",
    "expression": "$feature.type1 + $feature.type2 + $feature.type3",
    "returnType": "number"
  }]
})
```  

**Advanced Setting Content [[Demo](https://odoe.github.io/presentations/2018-PS-DevSummit/jsapi4-patterns-fundamentals/demos/widgets/popup-content-function.html)]**
```javascript  
popupTemplate: new PopupTemplate({
  content: getChart,
  title: function (event) {
    var graphic = event.graphic;
    return graphic.attributes.title;
  },
})
```

**Promises [[Demo](https://odoe.github.io/presentations/2018-PS-DevSummit/jsapi4-patterns-fundamentals/demos/widgets/popup-promises.html)]**  
```javascript  
view.popup.open({
  promises: [promise1, promise2, promise3],
  location: event.mapPoint
});
```  

#### ArcGIS Platform  
* Redesigned to [Portal API](https://developers.arcgis.com/javascript/latest/api-reference/esri-portal-Portal.html)  
* Access portal information: basemaps, featuring content.
* Query items, users, groups.  
* Load items (layers, webmap, webscene)  
* Create, delete, and update items.  

**Load a `WebScene`**:  
```javascript  
const scene = new WebScene({
  portalItem: {
    id: "082c4fd545104f159db39da11ea1e675"
  }
});

const view = new SceneView({
  map: scene,
  container: "viewDiv"
});
```  

**Loading a layer [[Demo](https://developers.arcgis.com/javascript/latest/sample-code/sandbox/index.html?sample=layers-portal)]**  
```javascript  
const promise = Layer.fromPortalItem({
  portalItem: {
    id: '8444e275037549c1acab02d2626daaee',
    portal: {
      url: 'https://myorg.maps.argis.com'
    }
  }
})
.then(layer => {
  // Adds the layer to the map once it loads
  map.add(layer);
})
.otherwise(error => {
  //handle the error
});
```  

**Portal items [[Demo](https://developers.arcgis.com/javascript/latest/sample-code/sandbox/index.html?sample=portalitem-dragndrop)]**  
```javascript  
const portal = new Portal();

// Setting authMode to immediate signs the user in once loaded
portal.authMode = 'immediate';

// Once loaded, user is signed in
portal.load()
  .then(() => {
    // Create query parameters for the portal search
    const queryParams = new PortalQueryParams({
      query: 'owner:' + portal.user.username,
      sortField: 'numViews',
      sortOrder: 'desc',
      num: 20
    });

    // Query the items based on the queryParams created from portal above
    portal.queryItems(queryParams).then(createGallery);
  });
```  

#### Interactivity with Input Manager  
* Use view events to interact with the view.  
* [List of events](https://developers.arcgis.com/javascript/latest/api-reference/esri-views-MapView.html#events-summary)  
* You can stop the propagation of the event to prevent the default behavior.  

**Drag [[Demo](https://odoe.github.io/presentations/2018-PS-DevSummit/jsapi4-patterns-fundamentals/demos/view/drag.html)]**  
```javascript  
view.on("drag", event => {
  // user won't be able to drag
  event.stopPropagation();
})
```    

**View Events [[API Sample](https://developers.arcgis.com/javascript/latest/sample-code/view-hittest/index.html), [Demo](https://odoe.github.io/presentations/2018-PS-DevSummit/jsapi4-patterns-fundamentals/demos/view/onclick.html)]**  

```javascript  
view.on("click", ({ x, y }) => {
  const screenPoint = {x, y};
  view.hitTest(screenPoint)
    .then(response => {
       // do something with the result graphic
       const graphic = response.results[0].graphic;
    });
});
```  

**View goTo() [[Demo](https://odoe.github.io/presentations/2018-PS-DevSummit/jsapi4-patterns-fundamentals/demos/view/goTo.html)**:  
Sets the view to a given target. Navigate to a geometry/feature/location.

**Collections [[Documentation](https://developers.arcgis.com/javascript/latest/api-reference/esri-core-Collection.html), [Demo](https://odoe.github.io/presentations/2018-PS-DevSummit/jsapi4-patterns-fundamentals/demos/collection/collection.html)]**:  
`esri/core/Collection`

#### Working with Accessor  
Objects are have properties that can be:  
* read and set  
* or read-only  
* constructor arguments  
* watchable  

**Property access**:  
```javascript  
console.log(layer.opacity);
console.log(layer.title);

layer.opacity = 0.5;
layer.title = "My test layer";

// setting multiple values
layer.set({
  opacity: 0.5,
  title: "My test layer"
});

// accessing the value of a deep property
view.get("map.basemap.title");
view.set("map.basemap.title", "new title");
```  

**Property watching [[Documentation](https://developers.arcgis.com/javascript/latest/api-reference/esri-core-watchUtils.html)]**:   
```javascript  
mapView.watch("scale", (newValue, oldValue, property, target) => {
  console.log(`scale changed: ${newValue}`);
});


mapView.watch("map.basemap.title", (newValue, oldValue, property, target) => {
  console.log(`new basemap title: ${newValue}`);
});


mapView.watch("ready, stationary", (newValue, oldValue, property, target) => {
  console.log(`property ${property}: ${newValue}`);
});

watchUtils.whenTrue(view, "stationary", () => {
  console.log("view is stationary");
})
```  

**Autocasting and Single Constructor**:  
```javascript  
// 4.x
  {
    type: "simple-marker",
    style: 'square',
    color: 'red',
    size: 10,
    outline: {
      color: 'rgba(255, 255, 255, 0.5)'
      width: 4
    }
  });

  // 3.x
  new SimpleMarkerSymbol(SimpleMarkerSymbol.STYLE_SQUARE, 10,
    new SimpleLineSymbol(SimpleLineSymbol.STYLE_SOLID,
    new Color([255,0,0]), 4),
    new Color([255,255,255,0.25]));
```  

**Autocast with Collections [[Demo](https://odoe.github.io/presentations/2018-PS-DevSummit/jsapi4-patterns-fundamentals/demos/collection/autoCast-collection.html)]**   


#### Promises  
* All asynchronous methods return a promise, no more events. For example:  
```javascript  
layer.queryFeatures(query).then(handleResult).catch(handleError);
```  
* Classes may be Promise
* Load resources
  * Asychronously initialized `Layer`, `WebMap`, `WebScene`, `View`.  
  * `view.then()` replaces `map.on('load', ...)`.  
  * Added `when()` to the API:

```javascript  
const map = new Map({...})

view = new SceneView({
  map: map,
  //...
});

view.when(() => {
  // the view is ready to go
});
```  

**Async/Await**:  
Work with native promises:  
```javascript  
const doQuery = async (query) => {
  const results = await layer.queryFeatures(query);
  const transformedResults = results.map(transformData);
  return transformedResults;
}
```  

**Chaining [[API sample](https://developers.arcgis.com/javascript/latest/sample-code/chaining-promises/index.html)]**:  
```javascript  
view.when(() => {
  return view.whenLayerView(map.findLayerById("awesomeLayer"));
})
.then(layerView => {
  return watchUtils.whenFalseOnce(layerView, "updating");
})
.then(result => {
  const layerView = result.target;
  return layerView.queryFeatures();
})
.then(doSomethingWithFeatures)
.catch(errorHandler);
```  

#### Loadables  
* Brings better control, and scheduling of loading resources.  
* Extension of `esri/core/Promise`.  
* In 3.x, instanciating a layer loads it. In 4.0, it's an explicit call.  
* The views automatically loads the map and its layers.  
* `WebMap` / `WebScene` need to load: [1] the portal item, [2] the layer module, [3] the layer's item.  
* `MapView` / `SceneView` need to load: [1] the map, [2] the layers.  

```javascript  
//In a single page application, get a feature from a FeatureLayer from a WebMap without displaying it, ASAP!
const webmap = new WebMap({
  portalItem: {
    id: 'affa021c51944b5694132b2d61fe1057'
  }
});

webmap.load()
  .then(() => {
    return webmap.getLayer('myFeatureLayerId').load();
  })
  .then(featureLayer => {
    return featureLayer.queryFeatures({
      where: 'OBJECTID = 1'
    });
  })
  .then(result => {
    displayDetails(result.features[0]);
  })
  .otherwise(error => {
    console.error(error);
  });
```  

## Wednesday, March 7, 2018

### Name of Presentation

## Thursday, March 8, 2018

### Name of Presentation

## Friday, March 9, 2018

### Name of Presentation
