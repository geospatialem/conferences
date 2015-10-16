# NACIS 2015 (Minneapolis, Minn.)

<img src="https://cloud.githubusercontent.com/assets/5023024/10469596/28626068-71cc-11e5-930d-dc6d5a3944f7.png" width="25" height="25")> [NACIS](http://www.nacis.org) is an annual conference facilitating communication in the map information community. There were a variety of talks focusing on the theme of *Mapping Interactions*.

## Sessions:

**Wednesday, October 14th, 2015:**  
* [Practical Cartography Day](#practical-cartography-day), Multiple speakers  

**Thursday, October 15th, 2015:**  
* [Examining the Terminology of Modern Cartography](#), Michael P. Peterson, Rex G. Cammack
* [A Visual Search Task Comparing Zooming Metaphors](#), Ryan Mullins
* [A New Atlas of American History](#), Alan McConchie
* [Beyond Paper: Ideas for Interactive Maps](#), Peter Liu
* [Open Web Mapping Technologies: How do we Teach this Stuff?](#), Carl Sack
* [How to Teach an Old(ish) Cartography Professor New Tricks](#), Sally Hermansen
* [Type on Maps: All the Little Things that Actually Matter](#), Elaine Guidero
* [Every Pixel Counts: Web Map Symbols for the National Park Service](#), Jake Coolidge
* [Visualizing Ten Years of Quantitative Color Schemes](#), Travis White
* [Natural-Color Maps via Automated Coloring of Bivariate Grid Data](#), Jane Darbyshire
* [Spooky Map Stories](#), Patrick Hammons
* [GIS for the people by the people](#), Sam Matthews

**Friday, October 16th, 2015:**  
* [Big History, Little History: Cartography in the Twentieth Century](#), Mark Monmonier
* [Of Crocodiles and Tea Garden Managers: Mapping Interactions of an Earlier Era](#), Leo Dillon
* [Improving ArcGIS mapping workflows with Adobe’s Creative Cloud Applications](#), Clint Loveman
* [Drupalized Web Maps](#), Tim Stallmann
* [Planning for Automated Labeling of U.S. Routes with Multiple Shields and Names](#), Cynthia A. Brewer
* [Cartography Driven Data Collection](#), Mamata Akella


**Saturday, October 17th, 2015:**
* [Mapping in the Cloud](#), Michael P. Peterson




## Wednesday, October 14th, 2015
### Practical Cartography Day

#### *Taking Terrain to New Heights with ArcGIS*, Kenneth Field & Patrick Kennelly [Story Map Presentation](http://www.arcgis.com/home/item.html?id=4b2ea7c5f87d476a8849c804b81667aa), [Resource](http://blogs.esri.com/esri/arcgis/2015/05/21/take-your-terrain-mapping-to-new-heights), [Download ZIP File](http://www.arcgis.com/home/item.html?id=4b2ea7c5f87d476a8849c804b81667aa)
* 13 different tools available [e.g. Sky modeled hillshade (sun, lowercast), shadow lines, different strokes, etc.]
* Takes some time to run, but is worth the wait.
* Works with 10.3+ (usually 10.2 as well). Although, choropleth has issues with older versions
* Samples are located in the download.

#### *Redesigning Atlas Maps for Social Media*, Alethea Steingisser and James Meacham
* Check out atlas work by Oregon, in particular the *Atlas of Wildlife Migration*  
* Real time engangement on social media using a "time series" highlighting particular areas of interest on-the-fly (esp. graphics, maps in HD). Bright colors, bold text, thicker outlines.
* Tell a story, what are you trying to tell? People will follow! (**give data a face**).
* Show the obstacles.
* Go bold - larger (and heavier) labels, heavier text, vibrant colors, and increased contrast.
* Simplify without 'dumbing down'.
* Use higher resolution than recommended (doubled in their work).

#### *MAPPublisher at National Geographic*, Matthew Chwatstyk
* Import, manipulate, analyze, edit, save vector data.
* Track data sources with a quick reference
* Plugin for Illustrator that can create themes depending on the use.

#### *A Quick Guide to US Dept. of Transportation Datasets*, Justyna Goworowska
* **Lots of spatial data** (e.g. NTAD 2015, also an atlas)
* WMS: http://gis.rita.dot.gov/ArcGIS/rest/services (download also available).
* Coordination with many other agencies to get other datasets.
* Web mapping/map tools available that includes data from multiple Federal agencies [Cyclist/pedestrian crash maps (?)].
* Contact [e-mail address](mailto:Justyna.Goworowska@dot.gov)

#### *Manual Shaded Relief of the World and the Patterson Projection*, Tom Patterson [Website](http://www.shadedrelief.com)

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

#### *Designer as a Cartographer*, Amy Lee Walton
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


#### *Collecting Data from the Crowd - A Leaflet and CartoDB-based Stack*, Mike Foster](@mjfoster83) [Slides](http://mjfoster83.github.io/nacis-2015)
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

#### *Dropchop*, Sam Matthews [Slides](http://bit.ly/nacisdropchop), [Website](http://chopchop.io), [GitHub](https://github.com/cugos/dropchop)
Make a simple modular tool (similar to: Geojson.io, Mapshaper, Turf.js, etc.)

**Hypothesis:**
1. GIS doesn't always require a server.
2. GIS can be *data-first*, not operation-first.
3. GIS is open (created and used by the community).

Query the OSM database (Query the overpass).  
*Note*: Refresh currently loses all work

#### Seth Fitzsimmons, *Practical and Impractical Uses of Terrain Data* (National Geographic Climate Change 'The Human Impact' example), [Slides](https://speakerdeck.com/mojodna/print-cartography-in-a-multi-resolution-world)

**Project Goals**:
* Re-purpose art, research, editorial, maps
* Make them interactive
* Make them multilingual

**Tell a story!!** It doesn't have to be in map form, think graphics that support your text. *You don't need to make a web map to write your story everytime.* Content is the most critical piece, get good content together.

**Anatomy of a ~~Web Map~~ Multi-resolution image**:
* 256 x 256 pixels tile
  * Scale up the images by 2 (512 x 512 pixels), to scale down.
* Tools: TileMill and After Effects (React and Leaflet)

#### *Mapping the Future Patagonia National Park*, Ross Donihue
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

#### *ArcMap-to-Illustrator Workflows*, Nicole Samu
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


#### *FixWikiMaps Project: Maplift*, [Brian Davidson](http://www.twitter.com/brianddavidson) [Twitter](http://www.twitter.com/fixwikimaps), [Website](http://fixwikimaps.github.io)
Maps need a lift!

**What can I do?**
1. Find a map, add it to the MapLift database
2. Claim a map
3. Create a map

#### *Restyling Old and Cluttered Maps*, Vanessa Knoppke-Wetzel
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

#### *Terrain Data Sources Online*, Paulo Raposo [Slides](http://1drv.ms/1rrsabo)
Uses SAGA for GIS. Also works with QGIS tools.

#### *A Matter of Perspective*, Daniel P. Huffman
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

#### *CartoCSS Essentials*, [Katie Kowalsky](http://www.twitter.com/katiekowalsky) [Slides](http://slides.com/kkowalsky/nacis-2015)

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

#### *Vector Cartography in ArcGIS*, Craig Williams  [Slides](https://speakerdeck.com/williamscraigm/nacis-2015-pcd-vector-cartography-in-arcgis)
ArcGIS vector tile service will come with the new release.

## Thursday, October 15th, 2015
### Rethinking Web Cartography

#### *Examining the Terminology of Modern Cartography*, Michael P. Peterson, Rex G. Cammack

**Words and Maps**:  
* Conceptually cartography is based on Words
* Words influence our mapping
* Words form communication with others, and **ourselves**
* Development of words done without much thought (expressions/words used for same concept).
* We're at a great age of cartography with **ideas, concepts, and theory.**
* Words to define cartography. Cartographic language is not a dead language.
* We as a community can change and help it evolve.
* *We need to find new words for other maps, and find a better term than "static map"!*

**Jargon**:
* Discipline-specific words (e.g. Doctors - shorthand/seperate from patients)
* Jargon separates out from individuals/groups

**Slippy map**:
* A term referring to modern web maps that let you zoom and pan around (map slips around when you drag the mouse).
* AJAX component where JavaScript runs in the browser and puts in a request from the server without downloading the whole HTML on the page -> "Slippy zoom" map experience - :-)
* A "cute" term, but not very professional sounding, and the term isn't taken very seriously.
* *MOMM (Me On My Map)* - Track the entity "holding" the map. Similar to slippy map term (e.g. FitBit)

**English by non-native speakers**:
* Worlds most spoken language? *bad english*
* Europeans use English as a common language, but words are made up (e.g. "Handy" in Germany, for cell phone)

**Boundaries of Classes**:
* Map Types (General/Thematic)
* Hybrids? (e.g. When does a "Labordoodle" become a "breed", do we use mashup names)?

#### *A Visual Search Task Comparing Zooming Metaphors*, Ryan Mullins, [Slides](https://speakerdeck.com/ryanmullins/geographic-analysis-in-context-a-visual-search-task-comparing-zooming-metaphors)
**Context:**
* The interaction between human and physical components.
* *How does context shape decisions and actions?*

**Metaphors**:
1. *Slippy map style*
  * Pinch-to-zoom basemap
  * Layer toggles in title bar
2. *Zoom window with toggles* (the worst rated)
  * No zoom on basemap
  * Pinch-to-zoom in windows
  * Layer toggles in zoom window
3. *Side-by-side zoom window*
  * No zoom on basemap
  * Pinch-to-zoom in windows
  * 1 window per layer, same footprint.

**Balance benefits**:
The best modality depends on the display size (slippy for smaller, side-by-side for larger screens), and the number of collaborating analysts. However, the results of the study were as follows:

1. *Slippy map*
  * Best performance (shortest time/most accurate)
  * Most familiar interaction
  * Zoom means different context
2. *Side-by-side zoom windows*
  * Second best performance (lowest varience)

#### *A New Atlas of American History*, Alan McConchie, [Slides](https://speakerdeck.com/almccon/a-new-atlas-of-american-history-nacis-2015), [Notes/Resources](http://sta.mn/6gk), [Website](http://dsl.richmond.edu/historicalatlas), [GitHub](http://github.com/americanpanorama)
*Showing things over time, is just as important as showing what is happening in space.*

**Notes**:
* Its hard to do, but its an important story to tell.
* Discuss!

**American Panorama: An atlas of U.S. History**:
* Don't build components (originally asked for), let's design from what the user will want. True to the data, and show a story. Add a toolkit over time. Use modern tools that support for many years.

**Forced Migration of Enslaved People in the US (1810-1860)**:
*Phases* (see photo)
* Let the user explore the story as they choose to.
* As you interact with the map, the URL changes appropriately so it can be shared as you are looking at it. *THIS IS AMAZING!*
* Setup (*see photo*)
* *Custom basemap:* Natural Earth data (cartoCSS/cartoDB), own map projection, transform using cartoCSS, openTerrain tile (mostly transparent).
* *Data:* Convert counties to hexbins that creates a smooth look (since counties change over time).

**Other maps**:
* Overland trails (1840-1860) - this includes historical trails (e.g. Oregon Trail)
* Foreign born ("current age" map)
* Canals (1820-1890)


#### *Beyond Paper: Ideas for Interactive Maps*, [Peter Liu](http://www.twitter.com/chieflybrit), [San Francisco Transit Solution Example](http://allthebuses.com), [Elevation Example](https://www.mapbox.com/blog/dc-bikeshare-revisited), [Time Travel Sled Race Example](https://www.mapbox.com/blog/playback-the-iditarod-with-turf), [E-mail](mailto:peter@mapbox.com)
*Interactive means we don't have to anticipate, only react when the user asks for information.*

**Breadth vs. Granularity** (*see photo*)
* Respond to user input
* Make it dynamic: show change over time

**Stories over time**
*Maps as an interface to discover information.*


### Web Mapping in Education

#### *Open Web Mapping Technologies: How do we Teach this Stuff?*, [Carl Sack](http://www.twitter.com/northlandiguana), [Slides](http://tinyurl.com/openwebmapping), [GitHub](http://github.com/uwcart/cartographic-perspectives), [Student Projects](http://geography.wisc.edu/courses/geog575)

**_Lots of great projects emerged, but so did the LARGE struggles, especially with D3._**

**Desired outcomes**:
1. Ability to create [animated] thematic slippy maps using Leaflet
2. Ability to created linked geovisualizations using D3
3. Independent completion of web map from start to finish in collaboration with colleagues.
4. Demonstration of computational thinking, adaptability, self-direction, and problem solving.
5. Integration of theoretical concepts presented in lecture into outcomes 1-3. (e.g. Human-map interaction, usability engineering, data visualizing, etc.)
  * This outcome was the hardest to meet.

**Web Mapping Workflow** (*Donahue, 2014*)  
The workflow gets more, and more, integrated over time.
1. Idea (Design)
2. Development environment
3. Data
4. Markup (representation space)
5. Script (interaction space)
6. Fine-tuning (usability)
7. Deployment

**Difficulties**:
* Two different sections (each has its own learnng speed)
* Difficulties: the DOM, identifying source of methods, data formatting and conversion.
* D3 lessons successful, exciting.
* Student understanding: "I'm learning and know I'll get beyond this rather than helplessness or giving up."
* Student enlightenment: "I needed to break it down and solve things one at a time, not all at once."
* Expertise with tools after were still low/moderate, but they had the basic knowledge and wanted to learn more!

**The most useful tools first were**:
* Using browser developer tools
* Tools on GitHub (mostly using GitHub GUI due to familiarity with command line. This can always come later.)

#### *How to Teach an Old(ish) Cartography Professor New Tricks*, Sally Hermansen, [Course: Research in Cartography (blog)](http://blogs.ubc.ca/advancedcartography)

**How/Why**:
* With 5 lines of code, we can make a map!
* But, what about a more refined map?
  * Joey Lee
  * Ben Fry: *Data Visualization Pipeline*
* Teaching Adobe Illustrator and ArcGIS is a diservice, they need to understand other tools/options in the open source community (Q, R, Leaflet, OSM, etc.)

**How it works**:
* Take students out of computer labs, bring their own laptops.
* GitHub tutorials
* Assignments outside of class, bring questions to class
* Videos during class, and work time

#### *Type on Maps: All the Little Things that Actually Matter*, Elaine Guidero
"Maybe Comic Sans isn't the best font for mapping a sex God."

**Typefaces**:
* Typefaces have different tones based on the semantic effects.
* Different semantic effects.

**Font anatomy** (*see photo*)

**Microaesthetics**:
* Differences (why?) - terminal, spur, serif, stroke contrast, ear, story,
* Looking for aesthetics, check out the photo for importance.
* Cartographic research on type aesthetics is inaccurate.
  * Why? B/c Label properties != typeface attributes.

(serif style, terminal style, x-height)

**Macroaesthetics (aka. Label properties)**:
* Spline/tilt
* Kerning/tracking

**Return to this section**:
Choose typeface:
* Use Microaesthetics...

Semantic effects (8)

Identify letters and earmarks

**Conclusions**:
* Letterform elements, not label properties, contribute to typeface tone.

#### *Every Pixel Counts: Web Map Symbols for the National Park Service*, [Jake Coolidge](http://www.twitter.com/jccartography)

**Design Considerations**:
* Recognizability (of symbols)
* Legibility
* Complexity (not too simplistic, but not too complex)
  * See Joshua Stevens' paper
* Style, or look and feel


#### *Visualizing Ten Years of Quantitative Color Schemes*, Travis White
Qc: Quantitative color schemes (color that represents quantitative data)

**Results**: 2004: 11% vs 2013: 71% used Qualitative color schemes

#### *Natural-Color Maps via Automated Coloring of Bivariate Grid Data*, Jane Darbyshire
Goal: Automate color technique for deployment to the web.

* Texture substitution

#### *Spooky Map Stories*, Patrick Hammons, [Slides](http://bit.ly/spooky-nacis-2015)

*Notes coming soon*

#### *GIS for the people by the people*, Sam Matthews, [Slides](http://bit.ly/gisforthepeople)

*Notes coming soon*

#### *Big History, Little History: Cartography in the Twentieth Century*, Mark Monmonier

**The History of Cartography**:
* J.B. Harley (1932-91)
* David Woodward (1994-2004)

**Modes of Cartographic Practice**:
* Overhead imaging
* Dynamic cartography
* Multi-mode institutions (academic cartography)

**Six themes**: (*need slides*)
1. Diverse impacts of mapping on a society
2. Overhead imaging
3. ...

**Books to read**:
* *Computational geography as a new modality* by Suane Marble
* *Cartogaphy in the Twentieth century*

#### *Of Crocodiles and Tea Garden Managers: Mapping Interactions of an Earlier Era*, Leo Dillon

**Observations**:
Lots of detail, and text describing the area as its explored.
* 1779 map (beavers on a map - where you can make money)
* 18xx St. Anthony's Falls (582 rabbits?)
* 1900: Number for each parcel
* Crocodiles
* Grave sites
* Tristan de Cunha ([original](http://www.britishempire.co.uk/images3/tristandacunha1937map.jpg))
* Evasion chart (EVC)

#### *Improving ArcGIS mapping workflows with Adobe’s Creative Cloud Applications*, Clint Loveman

#### *Drupalized Web Maps*, Tim Stallmann

#### *Planning for Automated Labeling of U.S. Routes with Multiple Shields and Names*, Cynthia A. Brewer

#### *Cartography Driven Data Collection*, Mamata Akella
