# Building with Bootstrap: Girl Develop It, July 2016 (Roseville, Minn.)

<img src="https://cloud.githubusercontent.com/assets/5023024/10260841/9d4cb9b8-6944-11e5-8987-a7d1493b5812.jpeg" width="25" height"25"> [Girl Develop It](https://www.girldevelopit.com/chapters/minneapolis) is a non-profit organization that exists to provide affordable and judgment-free opportunities for women interested in learning web and software development. Through in-person classes and community support, Girl Develop It helps women of diverse backgrounds achieve their technology goals and build confidence in their careers and their every day lives.  

## Course Instructors:  
Claire O'Neill, [[Slides](https://gdiminneapolis.github.io/building-with-bootstrap)]  

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
<img src="images/responsive-circle.jpg" alt="An example of a responsive circlular image" class="img-responsive img-circle">    
```  

See the [documentation](http://getbootstrap.com/css/#images) for more information.  

## Placeholder Images  
Some awesome resources to use placeholder images include:  
* [Placehold.it](http://placehold.it) (e.g. http://placehold.it/200x200)  
* [Place Kitten](http://placekitten.com) (e.g. http://placekitten.com/200/200)   

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

## Text Placeholders  
Some awesome resources to use placeholder text include:  
* [Loren Ipsum](http://www.lorenipsum.com)  
* [Hipsum](http://hipsum.co)    
* [Cupcake Ipsum](http://cupcakeipsum.com)    

## Awesome Text Editor Tidbits  
* Scroll to line #: `control` + `G`.  
* Edit multiple lines in Atom/Sublime: `⌘/command` + Click line(s).  
