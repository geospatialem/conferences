# NACIS 2015 (Minneapolis, Minn.)

<img src="https://cloud.githubusercontent.com/assets/5023024/10469596/28626068-71cc-11e5-930d-dc6d5a3944f7.png" width="25" height="25")> [NACIS](http://www.nacis.org) is an annual conference facilitating communication in the map information community. There were a variety of talks focusing on the theme of *Mapping Interactions*.

## Sessions:

**Wednesday, October 14th, 2015:**  
* [Practical Cartography Day](#practical-cartography-day), Multiple speakers  

**Thursday, October 15th, 2015:**  
* [Thursday Session Name Example](#), Speaker name  

**Friday, October 16th, 2015:**  
* [Friday Session Name Example](#), Speaker name

**Saturday, October 17th, 2015:**
* [Mapping in the Cloud](#), Michael P. Peterson


## Wednesday, October 14th, 2015
### Practical Cartography Day

#### Kenneth Field + Patrick Kennelly, *Taking Terrain to New Heights with ArcGIS*, [Story Map Presentation](http://www.arcgis.com/home/item.html?id=4b2ea7c5f87d476a8849c804b81667aa), [Resource](http://blogs.esri.com/esri/arcgis/2015/05/21/take-your-terrain-mapping-to-new-heights), [Download ZIP File](http://www.arcgis.com/home/item.html?id=4b2ea7c5f87d476a8849c804b81667aa)
* 13 different tools available [e.g. Sky modeled hillshade (sun, lowercast), shadow lines, different strokes, etc.]
* Takes some time to run, but is worth the wait.
* Works with 10.3+ (usually 10.2 as well). Although, choropleth has issues with older versions
* Samples are located in the download.

#### Alethea Steingisser and James Meacham, *Redesigning Atlas Maps for Social Media*
* Check out atlas work by Oregon, in particular the *Atlas of Wildlife Migration*  
* Real time engangement on social media using a "time series" highlighting particular areas of interest on-the-fly (esp. graphics, maps in HD). Bright colors, bold text, thicker outlines.
* Tell a story, what are you trying to tell? People will follow! (**give data a face**).
* Show the obstacles.
* Go bold - larger (and heavier) labels, heavier text, vibrant colors, and increased contrast.
* Simplify without 'dumbing down'.
* Use higher resolution than recommended (doubled in their work).

#### Matthew Chwatstyk, *MAPPublisher at National Geographic*
* Import, manipulate, analyze, edit, save vector data.
* Track data sources with a quick reference
* Plugin for Illustrator that can create themes depending on the use.

#### Justyna Goworowska, *A Quick Guide to US Dept. of Transportation Datasets*
* **Lots of spatial data** (e.g. NTAD 2015, also an atlas)
* WMS: http://gis.rita.dot.gov/ArcGIS/rest/services (download also available).
* Coordination with many other agencies to get other datasets.
* Web mapping/map tools available that includes data from multiple Federal agencies [Cyclist/pedestrian crash maps (?)].
* Contact [e-mail address](mailto:Justyna.Goworowska@dot.gov)

#### Tom Patterson, Bernhard Jenny, Bojan Savric, *Manual Shaded Relief of the World and the Patterson Projection*, [Website](http://www.shadedrelief.com)

**Manual Shaded Relief**:
* Better, small-scale manual relief shading.
* Check the data, verify its in the right location (older map topographies aren't so accurate).
* Use relief as a backdrop to your maps.
* Digital vs. Manual Relief comparisons.
* Digital: Light can make it difficult (e.g. Alaska arc and Pacific Northwest area), mountain ranges, gorges
* Terrain data: Natural Earth website (1:50m), can use higher/lower scales (GeoTIFF format).

**Patterson Projection**:
* Equal Area: Antartica is smooshed
* Geographic: "Stubby" South America
* Mercator: Small-scale = good, large-scal = not so much
* Miller: Antartica is a beast! (14x larger than Greenland)
* Patterson: Right in the middle**_!_**
  * Miller Projection was used as a template (*Compact Miller*)
  * Polar Compression to condense space around the poles.
  * Formula allows you to plug it into other sources (implemented in ArcGIS future release, and others). Made using Flexviewer (?)

**World Political Map**:
* World political map (e.g. Natural Earth, Natural Earth 2)

#### Amy Lee Walton, *Designer as a Cartographer*
* Cartographer's checklist:
  * What is the purpose?
  * Who is the audience?
  * What are the format?
* **Beauty and visability**
* Elements of Good Design
  * Heirarchy,
  * Color/Texture,
  * Typograpy,
  * Narrative
* Give visual form to an action, intention, material object, or narrative. (Data and inspiration).
* Examples:
  * **[AllTrails](http://alltrails.com)**: MapBox vector tiles for terrain using Mapbox Studio Classic. Filter to height, and zoom level.
  * **USS Enterprise Blueprint tiles** (*see photo*)
* Digital vs. Print - Make it for both! (*super difficult*). Download tiles as a PNG from Mapbox to print/play with.
* Don't let software limit you, re-created in Mapbox Studio for WebGL. *Simplify the process.*


#### [Mike Foster](@mjfoster83), *Collecting Data from the Crowd - A Leaflet and CartoDB-based Stack*, [Slides](http://mjfoster83.github.io/nacis-2015)
**How do you teach geography and design to non-geographers?**
* Concepts and fundamentals manifest themselves through tools.
* **DUSPviz**: *Skills and tools* for better planning.

**[Web Map Workshop](http://duspviz.mit.edu/web-map-workshop)**
* 7-week course (see slides for details)
* Base level = 0!
* End goal: Create a [data collection application](http://duspviz.mit.edu/web-map-workshop/databases-leaflet-cartodb)

**Tasks**:
1. *Backend*
    * Spatial database - used CartoDB SQL API
    * Security matters: API key, username, table (security matters!)
    * PHP for security (hide credential information on the server)
2. *FrontEnd*
    * JavaScript and jQuery
    * Create an empty dataset in CartoDB, with a few test points (e.g. Data Collector)
    * Set up HTML document structure
    * Add data to Leaflet (and Leaflet draw)
    * Modal for data collection
    * Proxy to send collected data to CartoDB
    * View data! :-P
3. *Security*
    * Check PR to address the problem (*see slides for more information*)

#### Sam Matthews, *Dropchop*, [Slides](http://bit.ly/nacisdropchop), [Website](http://chopchop.io), [GitHub](https://github.com/cugos/dropchop)
Make a simple modular tool (similar to: Geojson.io, Mapshaper, Turf.js, etc.)

**Hypothesis:**
1. GIS doesn't always require a server.
2. GIS can be *data-first*, not operation-first.
3. GIS is open (created and used by the community).

Query the OSM database (Query the overpass).  
*Note*: Refresh currently loses all work

#### Seth Fitzsimmons + Alan McConchie, *Practical and Impractical Uses of Terrain Data* (National Geographic Climate Change 'The Human Impact' example), [Slides](https://speakerdeck.com/mojodna/print-cartography-in-a-multi-resolution-world)

**Project Goals**:
* Re-purpose art, research, editorial, maps
* Make them interactive
* Make them multilingual

**Tell a story!!** It doesn't have to be in map form, think graphics that support your text. *You don't need to make a web map to write your story everytime.* Content is the most critical piece, get good content together.

**Anatomy of a ~~Web Map~~ Multi-resolution image**:
* 256 x 256 pixels tile
  * Scale up the images by 2 (512 x 512 pixels), to scale down.
* Tools: TileMill and After Effects (React and Leaflet)

#### Ross Donihue, *Mapping the Future Patagonia National Park*
* Connect people with place!!
* We save the places we love. We love the places we know. Know and feel connected to places.
* Stories of a landscape, that gives places meaning.
* Mapping the invisible information, takes time but it adds richness and meaning! *People will feel more connected!*

**1. Colors**
  * Extract colors from a palette derived from photos adds realism to maps (bring it into Photoshop to get the colors).
  * To extract, smudge/blur and get an eye dropper to get the natural landscape color.

**2. Talk about your work!**
  * Watch the magic unfold.
  * New connections are formed.
  * Unexpected, unforgettable experience by talking!

**3. Audio Recordings**
  * As you do fieldwork record audio of your local collaborators.
  * Record something you might miss if you were in the office.

**4. Skeleton Maps**
  *  Geographic structure for storing local stories and meaningful information.
  * Mark on the maps specific information they *know*, but we may not being outsiders.
  * Incorporate the information into field notes, and maps.

#### Nicole Samu, *ArcMap-to-Illustrator Workflows*
ArcMap -> Illustrator process

**Export Notes**:
* When exporting from ArcMap, *ungroup layers* that are checked in the TOC.
* Remove transparencies
* Choose '*Vectorize layers with bitmap markers/fills*' in the export settings.

**Illustrator Notes**:
* Open AI File
* Delete clipping masks (Object > Clipping Masks > Delete)
* Ungroup layers in layer panel as-needed
* Delete layer called 'other'
* Rename and organize layers in a functional matter
* "Save as" Illustrator Template file (File > Save as > Ai Template) or copy/paste in place of existing file.
* Clipping masks
* Legend customization (align panel)
* Colors (stroke/fill, custom color library, color guide panel)
* Improve text
* Adding style (Appearance panel/graphic styles panel/symbols panel)
* Improve performance (simplify paths/"place" graphics instead of embedding them)


#### [Brian Davidson](http://www.twitter.com/brianddavidson), *FixWikiMaps Project: Maplift*, [Twitter](http://www.twitter.com/fixwikimaps), [Website](http://fixwikimaps.github.io)
Maps need a lift!

**What can I do?**
1. Find a map, add it to the MapLift database
2. Claim a map
3. Create a map

#### Vanessa Knoppke-Wetzel, *Restyling Old and Cluttered Maps*
Anyone can anything nicer! But... fast maps? We can still do better!

**Program Map Restyling** (an iterative process):  
1. Before map (*see Syria photo*)  
2. After map  
  * Smaller map (only the map there, by itself - FOCUS)
  * Color-coded table
  * Words to symbols
  * Colors and shapes were added in
  * Font hierarchy, less contrast for busy maps
  * Color palettes in Adobe Illustrator.

**Reference Restyling**:
Stylize > Inner Glow (Illustrator). Set the blur based on size (small, medium, large). Make sure they are matching throughout your work.
Double-click eyedropper

#### Paulo Raposo, *Terrain Data Sources Online*, [Slides](http://1drv.ms/1rrsabo)
Uses SAGA for GIS. Also works with QGIS tools.

#### Daniel P. Huffman, *A Matter of Perspective*
Take familiar things and show them in a new, and different way. Daniel's map will be located in the map gallery throughout the conference.

**Why**:
Make a map your personal story. Lake Michigan as a straight line, to show its importance.

**How**:
* A linear View (not new, just different. e.g. Minneapolis LRT lines)
* ArcMap > Illustrator
* Census data (choropleth)
* Break segments into rectangles, and stack them (using ridiculous math equations). Process of transforming coordinates into rectangles.
* Once everything is shown vertically, work on the styling.
* Vertical vs. Horizontal (web vs. print)

#### [Katie Kowalsky](http://www.twitter.com/katiekowalsky), *CartoCSS Essentials*, [Slides](http://slides.com/kkowalsky/nacis-2015)

**Goal**: Create tileset using CartCSS based off of art.

**Why teach a class**:
* Teach an unfamiliar medium (the web!)
* Introduce Mapbox Studio and CartoDB
* Get students familiar with programming (HTML/CSS/JS)
* Challenge students

**Tips and Tricks for Designing Tiles**:
1. *It's dangerous to go alone.* Plan ahead on your design and make a game plan.
2. *Mise en Place*: Organization first!
  * Multiple styleshets
  * Use globals!
  * Hack `Project.yml` for custom layers
3. *Attachments* (a.k.a. sublayer)
4. *Attributes* are awesome!
5. Never forget *where you came from...* (Use common operators, and labels)
6. *Have fun!*

#### Craig Williams, *Vector Cartography in ArcGIS*, [Slides](https://speakerdeck.com/williamscraigm/nacis-2015-pcd-vector-cartography-in-arcgis)
ArcGIS vector tile service will come with the new release.
