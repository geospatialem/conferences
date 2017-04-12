# Building with Bootstrap: Girl Develop It, July 2016 (Roseville, Minn.)

<img src="https://cloud.githubusercontent.com/assets/5023024/10260841/9d4cb9b8-6944-11e5-8987-a7d1493b5812.jpeg" width="25"> [Girl Develop It](https://www.girldevelopit.com/chapters/minneapolis) is a non-profit organization that exists to provide affordable and judgment-free opportunities for women interested in learning web and software development. Through in-person classes and community support, Girl Develop It helps women of diverse backgrounds achieve their technology goals and build confidence in their careers and their every day lives.  

## Course Instructor:  
Claire O'Neill, [[Slides](https://gdiminneapolis.github.io/building-with-bootstrap)]  

## Awesome Text Editor Tidbits  
* Scroll to line #: `control` + `G`.  
* Edit multiple lines in Atom/Sublime: `⌘/command` + Click line(s).  

## Definitions  
* **Front-end Framework**: A collection of flexible, production-ready HTML, CSS, and JavaScript that we can use when we develop websites and applications.   

## Introduction  
Bootstrap is a front end framework that helps speed up the development of responsive websites. It is responsive, which means that your HTML elements will respond to changes in screen size. Best of all, Bootstrap allows designers & developers of all levels to build sites quickly.  

## Files
* **Base CSS**: Global CSS settings, Styling for fundamental HTML elements such as tables, forms, buttons, and images, and the grid system.  
* **Components**: Styles for common reusable components (e.g. jumbotron, glyphicon, thumbnail, and progress bar components).  
* **JavaScript**: jQuery-based JavaScript plugins for interactive elements such as tooltips, modal windows, and carousels (e.g. Scrollspy plugin).    


## Grid System  
The grid system is based on a 12-column grid and uses CSS classes to decide the width of each HTML element they’re applied to:  

<img width="686" alt="bootstrap grid system" src="https://cloud.githubusercontent.com/assets/5023024/17278707/fbea3eb4-5728-11e6-8cae-3be36add3746.png">  

Where each element can take up between 1 and 12 columns worth of space:  
<img width="686" alt="bootstrap grid system" src="https://cloud.githubusercontent.com/assets/5023024/17278756/f03eccfa-5729-11e6-9563-476b8f658272.png">  


### Rules
1. Rows must be placed within a `.container` (_fixed-width_) or `.container-fluid` (_full-width_) for proper alignment and padding.  

2. Use `.row` elements to create horizontal groups of columns
Content should be placed within columns, and only columns may be immediate children of rows.  

For example:  
```html  
<!-- Fixed width example -->  
<div class="container">  
  <div class="row">  
    [CONTENT FOR ROW]  
  </div>  
</div>  
```  
```html  
<!-- Full width example -->  
<div class="container-fluid">  
  <div class="row">  
    [CONTENT FOR ROW]  
  </div>  
</div>  
```  
```html  
<!-- Horizontal groups example -->  
<div class="container">  
  <div class="row">
    <div class="col-md-6">
      [CONTENT FOR COLUMN #1]
    </div>
    <div class="col-md-6">
      [CONTENT FOR COLUMN #2]
    </div>
  </div>
</div>
```  

### Column Classes   
<img width="536" alt="Bootstrap column classes" src="https://cloud.githubusercontent.com/assets/5023024/17278789/0c8bc100-572b-11e6-8983-08f6d45a56e0.png">  

**For example:**  
If you want to have two 50% columns on a mobile phone, you would use `.col-xs-6` nested in a `.row`, and the rows would be consistent on every device.

<img width="535" alt="Bootstrap column example on mobile devices" src="https://cloud.githubusercontent.com/assets/5023024/17278797/79943840-572b-11e6-814b-303d417f7bd4.png">  


```html  
<!-- Column classes example -->
<!-- The columns will stay at 50% of the window all the way down to a mobile device. They will not break down to 100%. -->
<div class="container">  
  <div class="row">
    <div class="col-xs-6">
      [CONTENT FOR COLUMN #1]
    </div>
    <div class="col-xs-6">
      [CONTENT FOR COLUMN #2]
    </div>
  </div>
</div>
```  
**For example:**  
If you want to have four 25% columns on a desktop, and would like them to break to 100% on a tablet, you would use `.col-md-3` nested in a `.row`.  

<img width="535" alt="Bootstrap desktop column example" src="https://cloud.githubusercontent.com/assets/5023024/17278831/054f8844-572c-11e6-9e8c-6c2c60a44532.png">  

```html  
<!-- Column classes example -->
<!-- The columns will break down to 100% at 992px. -->
<div class="container">  
  <div class="row">
    <div class="col-md-3">
      [CONTENT FOR COLUMN #1]
    </div>
    <div class="col-md-3">
      [CONTENT FOR COLUMN #2]
    </div>
    <div class="col-md-3">
      [CONTENT FOR COLUMN #3]
    </div>
    <div class="col-md-3">
      [CONTENT FOR COLUMN #4]
    </div>
  </div>
</div>
```  

### Media Queries  
**Q:** _How is it doing that?_  
**A:** _It's magic!_  :smile_cat:  

Media query is a CSS technique introduced in CSS3. It lets you add breakpoints where certain parts of the design will behave differently on each side of the breakpoint. Bootstrap uses the breakpoints **768px**, **992px**, and **1200px**.  

 _**Note:**_ Check out the `pull` and `push` CSS classes in the Bootstrap documentation.  

## Images  
Images can be made responsive with `.img-responsive`, which adds `max-width: 100%` and `height: auto` to scale the image to its parent container.  

Other styling classes: `.img-rounded`, `.img-circle` (only functional on square images), and `.img-thumbnail`.  

For example:  
```html  
<!--Example of a responsive image-->  
<img src="images/responsive-image.jpg" alt="An example of a responsive image" class="img-responsive">   

<!-- Example of a responsive image given a circular shape -->  
<img src="images/responsive-circle.jpg" alt="An example of a responsive circular image" class="img-responsive img-circle">    
```  

See the [documentation](http://getbootstrap.com/css/#images) for more information.  

## Placeholder Images  
Some awesome resources to use placeholder images include:  
**[Placehold.it](http://placehold.it)** (e.g.   http://placehold.it/200x200):  
<img width="197" alt="Placeholdit example" src="https://cloud.githubusercontent.com/assets/5023024/17279204/414a0e16-5734-11e6-8a58-e0b9e245448d.png">  

**[PlaceKitten.com](http://placekitten.com)** (e.g. http://placekitten.com/200/200):     
<img width="197" alt="Placekitten.com example" src="https://cloud.githubusercontent.com/assets/5023024/17279195/1a75e79c-5734-11e6-89ea-738e0983543b.png">  

## Buttons  
The button class .`btn` can be used on `<button/>`, `<input/>`, or `<a/>` elements.  

Additional classes can be used to provide extra visual weight and identify primary button actions, such as: `.btn-default`, `.btn-primary`, `.btn-success`, and others!  

For example:  
```html  
<!-- Button example -->
<button class="btn btn-default">This is a button</button>  

<!-- Primary button with a link example -->
<a href="btn btn-primary">This is a link but it looks like a button</a>  
```

See the [documentation](http://getbootstrap.com/css/#buttons) for more information.  

## Navbar  
**Class example:**   
* Add a `<nav>` with the classes `navbar` and `navbar-default` inside a `<header>` element.  
* Add a `.container-fluid` to the `nav`.  
* Add a toggle button within the `nav` for mobile devices. Then add the `div` that has the classes `collapse navbar-collapse`, including the `<ul>`, and paste it as a sibling of the toggle button.  
* Finally, add three list items (`<li>`) with a link (`<a>`) inside each for the page sections to be used later.  


```html  
<header class="text-center"><!--center the text of an element with a header-->
  <nav class="navbar navbar-default navbar-fixed-top">
    <div class="container-fluid">

      <!--Hamburger menu button-->
      <button type="button" class="navbar-toggle collapsed" data-toggle="collapse" data-target="#navbar" aria-expanded="false">
        <span class="sr-only">Toggle navigation</span><!--Screen reader only-->
        <span class="icon-bar"></span>
        <span class="icon-bar"></span>
        <span class="icon-bar"></span>
      </button><!--/Hamburger menu button-->

        <!-- Collect the nav links, forms, and other content for toggling -->
        <!--Note: It **MUST** have same id tag as the data-target above to join them together-->
      <div class="collapse navbar-collapse" id="navbar">
        <ul class="nav navbar-nav">
          <li><a href="#nav1">Navigation Item #1</a></li>
          <li><a href="#nav2">Navigation Item #2</a></li>
          <li><a href="#nav3">Navigation Item #3</a></li>
        </ul>
      </div>

    </div>
  </nav>
</header>
```  

## Webpage Section  

### Text Placeholders  
Some awesome resources to use placeholder text include:  
* [Loren Ipsum](http://www.lorenipsum.com)  
* [Hipsum](http://hipsum.co)    
* [Cupcake Ipsum](http://cupcakeipsum.com)   

```html  
<!--Webpage section example-->
<section id="section-example">
	<div class="container">
			<div class="row">
				<div class="col-md-3"><!--title-->
					<h2>Section Example</h2>
				</div>
				<div class="col-md-9">
					<div class="row">
					<div class="col-sm-8">
						<img src="http://placekitten.com/g/300/300" class="img-responsive img-circle" alt="Responsive kitten circular image">
						<p>Drinking vinegar celiac paleo everyday carry locavore bushwick wolf. Leggings cliche fap, 3 wolf moon
							mlkshk YOLO +1 venmo keytar tousled drinking vinegar actually.</p>
					</div>
					<div class="col-sm-4">
						<!--<ul>--><!--Unordered & Styled list-->
						<ul class="list-unstyled"><!--Unordered & Unstyled list-->
							<li><span class="glyphicon glyphicon-phone" aria-hidden="true"></span>###-###-###</li>
							<li><span class="glyphicon glyphicon-envelope" aria-hidden="true"></span>mailme@mail.com</li>
							<li><span class="glyphicon glyphicon-globe" aria-hidden="true"></span>Location</li>
						</ul>
					</div>
				</div>
				</div>
			</div>
	</div>
</section><!--/Webpage section example-->
```

```html  
<!-- Webpage section example with similar elements -->
<section id="section-similiar-elements-example">
  <div class="container"><!--Bootstrap container-->
      <div class="row"><!--Bootstrap row-->
        <div class="col-md-3"><!--Section title-->
          <h2>Section Example with Similar Elements</h2>
        </div><!--/Section title-->
        <div class="col-md-9"><!--Sub-section containing similar elements-->          
          <div class="row"><!--Item #1-->
            <div class="col-md-3"><!--Header #1-->
              <h5>Header #1</h5>
            </div><!--/Header #1-->
            <div class="col-md-9"><!--Supporting content #1-->
              <h3>Sub-header #1</h3>
              <h4>Supporting sub-header #1</h4>
              <p>Supporting content #1</p>
            </div>
          </div><!--/Item #1-->      
          <div class="row"><!--Item #2-->
            <div class="col-md-3"><!--Header #2-->
              <h5>Header #2</h5>
            </div><!--/Header #2-->
            <div class="col-md-9"><!--Supporting content #2-->
              <h3>Sub-header #2</h3>
              <h4>Supporting sub-header #2</h4>
              <p>Supporting content #2</p>
            </div>
          </div><!--/Item #2-->
        </div><!--/Sub-section containing similar elements-->
      </div><!--/Bootstrap row-->
  </div><!--/Bootstrap container-->
</section><!--/Webpage section example with similar elements-->
```

## Progress Bars  

```html  
<!-- 100% progress bar example -->
<div class="progress">
  <div class="progress-bar" role="progressbar" aria-valuenow="100" aria-valuemin="0" aria-valuemax="100" style="width: 100%;"><!--The aria values are read to a screen reader, the width shows it visually-->
    <span class="sr-only">100% progress</span><!--Screen reader value-->
  </div>
</div>

<!-- 60% progress bar example -->
<div class="progress">
  <div class="progress-bar" role="progressbar" aria-valuenow="60" aria-valuemin="0" aria-valuemax="100" style="width: 60%;"><!--The aria values are read to a screen reader, the width shows it visually-->
    <span class="sr-only">60% progress</span><!--Screen reader value-->
  </div>
</div>
```

## Thumbnails  
Make an image a thumbnail using the `img-thumbnail` class.  

For example:  

```html  
<!--Responsive thumbnail example that is 1/3 the screen until small devices (100%). -->
<div class="col-sm-4">
  <img src="http://placekitten.com/g/800/800" class="img-responsive img-thumbnail" alt="Responsive thumbnail example">
  <h4>Responsive Thumbnail Example</h4><!--Thumbnail title-->
  <h5>Supporting text here</h5><!--Thumbnail details-->
</div>
```  

## Footer  

```html  
<footer><!--Footer-->  
 <div class="container text-center"><!--Center the div on the page-->  
   <small>&copy; 2016</small><!--Copyright text-->  
 </div><!--/div-->  
</footer><!--/Footer-->  
```    

## Scrollspy  
Scrollspy targets the links inside an element selected. One of the easiest and fastest ways to do that is to use an element’s ID.  For example, Scrollspy can enhance your webpage's navigation like so:  

![scrollspy-example](https://cloud.githubusercontent.com/assets/5023024/17279690/c0234a16-5740-11e6-83a6-a5e76d11f3db.gif)  

To initialize Scrollspy, the jQuery and Bootstrap libraries must be added to your .html file and the following JavaScript must be added:  

```javascript  
//Enable scrollspy using jQuery  
$('body').scrollspy({ //Use the html body in most cases (some exceptions apply)  
  target: '#navbar' //Target the element for Scrollspy to use (e.g. navbar)  
});  
```  

You can also add an `offset` option using the number of pixels you'd like to "offset" from the default pixels, like so:  
```javascript  
$('body').scrollspy({ //Use the html body in most cases (some exceptions apply)  
  target: '#navbar',//Target the element for Scrollspy to use (e.g. navbar)  
  offset: 150 //Pixels to offset from top when calculating position of scroll.  
});  
```  

See the [documentation](http://getbootstrap.com/javascript/#scrollspy) for more information.
