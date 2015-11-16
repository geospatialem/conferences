# Photoshop: Girl Develop It, November 2015 (Eagan, Minn.)

<img src="https://cloud.githubusercontent.com/assets/5023024/10260841/9d4cb9b8-6944-11e5-8987-a7d1493b5812.jpeg" width="25" height"25"> [Girl Develop It](http://www.midwestjs.com) is a non-profit organization that exists to provide affordable and judgment-free opportunities for women interested in learning web and software development. Through in-person classes and community support, Girl Develop It helps women of diverse backgrounds achieve their technology goals and build confidence in their careers and their every day lives.

## Introductions
* Presenter: [Karly Anderson](https://twitter.com/karlya8)
* [Presentation Slides](https://docs.google.com/presentation/d/1ggeVIvIU1zH0fcW5HAW6msI_pToQReHyTeV6Vkzy0YY)

## Vocabulary
* **_PSD:_** File extension for Photoshop files.
* **_Photoshop Elements_**: A good tool for photography, not as elaborate at Photoshop.  
* **_Raster:_** Dot/pixel-based graphics. Raster graphics cannot resize without quality loss. Photoshop uses raster graphics. Most commonly, rasters are in GIF, JPG, or PNG formats.     
* **_Vector:_**  Math-based, and uses geometry to create graphics. Infinitely resize or scale while maintaining a graphic's quality. Illustrator uses vector graphics. Most commonly, vectors are in SVG formats.  
* **_Pixel:_** Short form of two words, "picture element".  They are the building blocks of any digital photo or image.  
* **_Duplicate layer:_** A copy/duplicate of the original. **Note:** This is a best practice in Photoshop to keep existing files and edited files separated. Make this part of your workflow!
* **_Smart Guides:_** Align items more effectively while designing.
* **_Layer Mask:_** The capability to selectively modify the opacity (transparency) of the layer.  
* **_Layer adjustments_**: Apply color and tonal adjustments to an image without permanently changing pixel values.

## Raster vs. Vector
![raster-vs-vector](https://cloud.githubusercontent.com/assets/5023024/11166959/c8841af0-8b12-11e5-8311-c1d2ebbf07f0.png)

## Shortcuts
When in doubt, try the `Shift` or `⌘` keys.  

![shortcuts-1](https://cloud.githubusercontent.com/assets/5023024/11164448/16e0b3a0-8ab6-11e5-8c38-07db418a1f0f.png)

![shortcuts-2](https://cloud.githubusercontent.com/assets/5023024/11164449/16ec10f6-8ab6-11e5-9ed9-524dd0f2f144.png)

## Print vs. Web
* **Print**: CMYK  
* **Web**: RGB  

## File Types for Web [[Resource](http://www.espressographics.com/text/fileformats.html)]
1. **PNG:** PNG files allow transparency to be set on a scale between opaque and completely transparent, allowing for a faded, translucent look. Some older browsers may have trouble supporting PNG files because of alpha-channels. PNG images are of higher quality. *Best Uses:* Web images such as logos that involve transparency and fading, images in the middle of the editing process, and complex images like photographs if file size is not an issue.
  * **PNG-8:** Very similar to GIF - even smaller than GIF files with 256 colors and 1-bit transparency.
  * **PNG-24:** 24-bit color, similar to JPEG - Can include over 16 million colors. Lossless compression means larger files than JPEG.  

2. **JPEG/JPG:** A standard file format of digital cameras and web pages that can display millions of colors - although does not allow transparency. *Best Uses:* Still images, Real-world photos, and complex coloring/shading of light and dark.
  * Uses a very complex compression algorithm to reduce file size
  * Let image details be “forgotten” and then fill in when displayed
Called “lossy” compression for the lost data.
  * Use when a small file size is more important than maximum quality.

3. **GIF:** Uses 256 indexed colors through dithering, a process where two pixel colors combine to make one to reduce number of colors needed, also using lossless compression. Fewer colors means files start even smaller than JPEG. *Best Uses:* Web graphics with few colors, small icons, animations, and simple images.
  * Progressive loading shows a low-quality version first and then better detail is added.
  * Can be animated
  * Allows for single-bit transparency - one color can be chosen to be transparent.
  * Lower number of colors
  * Reuses colors throughout the image

![file-types](https://cloud.githubusercontent.com/assets/5023024/11164816/442405c8-8ac1-11e5-9301-2d459fd5a373.png)
Check out the [full infographic](http://www.whoishostingthis.com/blog/2014/12/06/jpeg-gif-png/).  

## Saving a File
* `⌘` +`S`
* `Save for Web` (*Legacy in Photoshop CC*), but recommended for optimization.
* [Export artboards, layers, and more](https://helpx.adobe.com/photoshop/using/export-artboards-layers.html), help article

## Key tools

### Exporting
* Leave the color profile as-is

### Zoom
* Zoom in: `⌘` +`+`
* Zoom out: `⌘` +`-`

### Rulers/Grids
* `Preferences → Units and Rulers...`
* `⌘` +`R`
* 960/1170 are the most commonly used
* There is a Bootstrap Flexible Column Grid!

### Guides
`View → Snap to`

### Magic wand
* Check out the `Sample size` drop-down menu
* Check out the `Tolerance` to select more/less within your project.
* Use `Reselect/Deselect`
* `Shift` adds a selection
* Utilize the `Select inverse` option

### Remove an area
`Alt/option` + `-`

### Lasso
Erasing is destructive, ensure you have made a duplicate layer, and/or are using an embedded image before proceeding.
* **Magnetic Lasso:** Differentiate between a person's head with a landscape background
* **Polygonal Lasso:** POLYGONS!

### Eyedropper/Color sampler

### Crop
* Photoshop remembers your settings, be sure to clear the settings, if necessary.
* Utilize different ruler/grid types.
#### Workflow:  
1. Crop the image to the extent desired.  
2. Change the image size to fit the need.  

### Image size `Image → Image size`  

### Hand  

### Rubber band  

### Drawing
* **Brush:** Many different sizes, styles, and hardness' (clarity) levels.  
* **Pencil:** Smaller, more precise, version of brush.  

### Pen (like Illustrator)  
* **Path**  
* **Shape**  
  * Vector-based  
  * Paths  
  * Pixel layers  
  * Create shapes with the pen tool, and save custom shapes by clicking on the shape `Define custom shape`.  
  * To create a circle, click and hold to go along a curve.
* **Path selection**  

## Layers and Layer Panels
* **Best Practices:** Copy the original image, and keep the background layer locked.
* **Layer mask:** Useful to remove content without deleting (do **_not_** delete content from the original file).
* **Link layers** together by combining two, or more layers and `link` them. This will keep the layers in sync with each other.
* **Layer Groups** group individual layers together. If you highlight the group, the group will respond similar to linked layers.

## Image Canvas Size
* **_Good for banners!_**
* Extend the canvas size
* The anchor is based on where you want it to **expand**.
* If you make the canvas size smaller than the current image size, it will crop the image.

## Embedded and Linked images [[Resource](https://forums.adobe.com/thread/1398884)]

### Linked images
Linked images are linked directly back to the original file. Any changes to the linked image will reflect back to the original file.

### Embedded Images
* Once embedded, click `enter`/`return`. The image is considered a *smart object*, meaning it can be edited within Photoshop, and will not alter the original image.

### Place
* Adjusts to one set of margins currently displayed in the document (either horizontal or vertical).
* Press `enter` to place the image.
* To resize the image, use **Transform**: `Edit → Transform → Scale`. While resizing, **_always hold down the `shift` key_** to maintain the original object.
* However, smart objects cannot be used in Photoshop until they are **rasterized** (you can always convert back). To rasterize, click `rasterize` on the smart object layer.

## Layer Styles
Also known as effects (e.g. color overlay, glow, etc.)

## Layer Mask
Layer masks are based on the opacity of brush effects.

### Workflow:
1. Open image
2. Embed another image
3. Ensure black is the primary color (white would show the entire image as-is).
4. Paint!

For example:  
![layer-mask](http://designshack.net/wp-content/uploads/masking101-3.jpg)

## Filters
Filter gallery contains a large majority of major filters, mostly artsy. The filter menu has a more comprehensive list of filters. You can also apply multiple filters and drag them around in your project.

## Type
* Point text vs. Paragraph text
* Crisp/Sharp
* Change text orientation (e.g. horizontal → vertical)
* Faux typing (imitated font uses, like italic)
* **Copy CSS**: `Layer → Copy CSS` You can remove `z-index` and `position` as they relate directly to Photoshop. **_(P.S. This is amazing!)_**   

## Blending Modes and opacity
* Normal
* Multiply (this one is *sweet*)
* Darken
* Screen
* Soft Light
* Overlay
* Lighten
* Contrast
* Inversion
* Cancellation
* Component

## Layer comps
Store everything to revert back, if needed. Particularly useful for different webpages, text levels, or prototypes.

### Saving
The following attribution is saved with Layer comps:
1. Layer visibility
2. Layer position
3. Layer appearance

### Exporting
`File → Export → Layer comps to files`

## Edit Background Fill
* `Edit → Fill`
* Content aware
* If you want to expand the image (copy/paste) into the picture.

## Other stuff to check out
* Cloning
* Check out libraries (new in CC)
* Explore files on the interwebs for inspiration!
