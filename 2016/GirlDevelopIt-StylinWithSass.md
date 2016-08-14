# Stylin' with Sass!: Girl Develop It, August 2016 (Minneapolis, Minn.)

<img src="https://cloud.githubusercontent.com/assets/5023024/10260841/9d4cb9b8-6944-11e5-8987-a7d1493b5812.jpeg" width="25" height"25"> [Girl Develop It](https://www.girldevelopit.com/chapters/minneapolis) is a non-profit organization that exists to provide affordable and judgment-free opportunities for women interested in learning web and software development. Through in-person classes and community support, Girl Develop It helps women of diverse backgrounds achieve their technology goals and build confidence in their careers and their every day lives.  

## Course Instructor:  
[Tamara Temple](https://twitter.com/tamouse), [[Slides](https://gdiminneapolis.github.io/html-320-stylin-with-sass)], [[Printed Slides with Comments](https://gdiminneapolis.github.io/html-320-stylin-with-sass/print.html)], and [[Project Files](https://github.com/gdiminneapolis/html-320-stylin-with-sass-project-files/archive/master.zip)]           

## Tips & Tricks  

### Command Line  
* Stop a terminal session: `control` + `C`  
* Watch Sass, compile CSS from Sass: `$ sass --watch stylesheets/scss:stylesheets/css`  
* Open a page: `open [index.html]` (does not work if a server is needed).  
* `pushd`: Saves the current working directory in memory so it can be returned at any time, optionally changing to a new directory.  
* `popd`: Returns to the path at the top of the directory stack.  
* `mkdir`: Make directory  
* Home directory  
* Listing files  


#### Home Directory    
```
cd # OR...
cd $HOME # OR...
cd ~ # that's a "tilde"  
```  

#### Listing Files  
```
ls # => shows non-hidden files in a table
ls -A # => shows hidden files as well
ls -Al # => shows all files in a
       # .. long format listing
```

### Task Runners  
* Make  
* [Rake](http://docs.seattlerb.org/rake)  
* [Grunt](http://gruntjs.com)  
* [Gulp](https://gulpjs.com)  
* [Webpack](https://webpack.github.io)    
* [npm scripts](https://www.npmjs.com/package/task-runner)  

### Resources  
* [Sass home page](http://sass-lang.com)  
* [Sass Documentation](http://sass-lang.com/documentation/file.SASS_REFERENCE.html)  
* [Cross-Browser CSS3 Gradients](http://codepen.io/cfarm/pen/jteAG)  
* [Cross-Browser Box-shadow (drop shadow) effects](http://codepen.io/cfarm/pen/rkEIo)  
* [Inner Text Shadow effect](http://codepen.io/andrewboyd/pen/LmIxi)  
* [Off-Canvas Responsive Layout](http://oddbird.net/demos/susy-off-canvas)  
* [Codepen.io](http://codepen.io)  

## What is Sass?  
Sass, or **S** -yntactically **A** -wesome **S** -tyle- **S** -heets, is a command-line tool that pre-processes your CSS files to allow you to create modular, DRY, and easily maintainable style information.  

Sass is a pre-compiler, and runs on your hardware to convert your **.scss/.sass** files into **.css** files that you can upload to your website's server. This requires an install of Ruby and Sass.

### Dialects
**Sass:** Stripped down, white-space indented, terse; does not look like CSS.

```scss
nav
  ul
    list-style: none
```

**SCSS:** Keeps all the braces (“squirly brackets”) and semi-colons that you have in CSS. White space doesn’t matter. Plain CSS is already SCSS, it’s the easiest to start with.  

```scss
nav {
  ul {
    list-style: none;
  }
}
```  

### Installation  
Install Ruby (usually installed on a Mac). If you need to install Ruby, follow the directions on their [website](http://RubyInstaller.org) based on your OS. To check on Mac if it's installed run the following command in Terminal: `$ ruby --version`.  

Once installed, on a Mac perform the following in Terminal:  

```
$ gem install sass --user-install
$ sass --version
```  

#### Path Variable
You'll need to add the Ruby location to your path variable. I used [this resource](http://code.tutsplus.com/tutorials/how-to-install-ruby-on-a-mac--net-21664) as a help guide. To do so on Mac OS, perform the following steps:   

In the command prompt:  
```
$ cd ~/
$ sudo vim .bash_profile
```  

You'll be asked to enter in your Mac OS password, enter it in.  

Next, you'll be using VIM. Enter in the following VIM commands:  
* Press `i` to insert text, at the bottom of the file.
* Add `export PATH="$PATH:$HOME/.gem/ruby/2.0.0/bin"`. Remember to swap in the correct ruby version (my example is version 2.0.0). To check your version type, you'll need a separate terminal session and run `$ ruby --version`.
* Once complete, press `esc`, and `:wq` to exit VIM.  

Once completed, close your terminal session and re-open it to refresh your settings and enter in `$ echo $PATH`. The newly created path should now be listed.

## Watch Command  
* The `--watch` option tells Sass to look for changes to our .scss files, and to compile them to css if they have updates.  
* The scss option is the folder where our .scss files live (stylesheets/scss).  
* The css option is the folder where our .css files will be.  
* Remember: We only edit the files under stylesheets/scss!  

For example:
```
$ sass --watch stylesheets/scss:stylesheets/css
```  


## Variables
Sass let’s you set variables that can hold values used all over your css files, allowing you to quick change a commonly used value in only one place. Variables are easy to change if you **keep them all in one stylesheet**, and update or add to the styles as needed. Sometimes you want to reuse a value for a style - you use them frequently, they’re hard to type or remember, such as:  
* Colors (e.g. #2a79af)  
* Font stack styles (e.g. Georgia, Times, Times New Roman, serif, etc.)  
* Font sizes (e.g. 1.667em)  

For example:  
```scss
header {
  color: $mainTextColor;
  background-color: $brandColor;
}
.content {
  color: $mainTextColor;
  background-color: $accentColor;
}
footer {
  color: $accentColor;
  background-color: $brandColor;
}
```
Sass input:  
```scss  
$brand-primary: seagreen;
$brand-accent: tomato;
$brand-bg: honeydew;
header {
  background: $brand-bg;
  color: $brand-primary;
}
header a { color: $brand-accent; }
```

CSS output:  
```css
header {
  background: honeydew;
  color: seagreen;}
header a {
  color: tomato;}
```  

### Colors  
```scss  
// Colors
$favoriteColor: #2a79af;
$anotherColor: #f05b62;
```   

### Fonts  
```scss  
// Font Stacks
$favoriteFont: Papyrus, fantasy;
$aPracticalFont: "Trebuchet MS",
  "Lucida Grande", "Lucida Sans Unicode",
  "Lucida Sans", Tahoma, sans-serif;

// Font sizes
$aNiceBigFontSize: 1.2em;
$finePrint: 9px;
$giantLogo: 36px;
```  

### Margins and Padding  
```scss  
$defaultMargin: 15px;
$defaultPadding: $defaultMargin;
```  


### Defining Variables  

Variables with Sass let us reuse values more than once, while only defining them in one place. Variables are easy to change if you keep them all in one stylesheet, and update or add to the styles as needed. To create a variable you need a dollar sign (`$`) before the name of your variable, and a colon (`:`) to give it a value.  

For example:  
```scss  
//define variable using dollar sign:  

$brandColor: #f90000;
$mainTextcolor: #fff;
$accentColor: #ccc;
```

### Commenting  
Note that in Sass files, you can comment out a line with two slashes (`//`), like so:  

```scss  
$brandColor: #f90000; // red
$mainTextcolor: #fff; // white
$accentColor: #ccc; // grey
```  

## Nesting  
Gives you the ability to condense your code and let you list your selectors using the same hierarchy you see in your HTML code. There is a caveat, however, in that you should not nest your selectors too deeply. Sass allows the nesting of CSS so you can clearly tell which rules apply to which parent, without endless repetition. _A good rule of thumb is to nest no more than **three levels** deep and use more specific selectors to target specific layout needs._   

Sass input:  
```scss  
header {
    color: black;
    nav {
        background: red;
        a { color: white; }
    }
}
```

CSS output:  
```css
header { color: black; }
header nav { background: red; }
header nav a { color: white; }
```  

## Parent Selectors  
Sometimes it’s useful to use a nested rule’s parent selector in other ways than the default. For example, you might want to have special styles for when that selector is hovered over or for when the body element has a certain class. In these cases, you can explicitly specify where the parent selector should be inserted using the & character.  

Sass input:
```scss
nav {
  background: red;
  a {
    color: white;
    &:hover { text-decoration: underline; }
  }
}
```

CSS output
```css
nav { background: red; }
nav a { color: white; }
nav a:hover { text-decoration: underline; }
```  

## Mix-ins  
**Declare, and reuse.** Mix-ins let you specify often repeated style specification that are used in several independent styles, similar to the way variables allow the reuse of values. They are quite useful for creating common settings for different elements and components to create a unified look and feel. You could consider a mix-in like a macro, where the mix-in’s content gets included in the style specification.   

They come in handy for CSS effects, such as:  
* Gradients  
* Drop shadows  
* Browser prefixes  
* Clearing floats    

For example:  
```scss
@mixin visually-hidden {
  text-indent: 100%;
  white-space: nowrap;
  overflow: hidden;
}
.image-replace {
  @include visually-hidden;
  background: url(logo.png) no-repeat;
}
```  

Sass input:  
```scss  
@mixin dropshadow($text) {
  color: $text;
  text-shadow: 2px 4px lighten($text, 40%);
}
h1 {
  @include dropshadow(black);
  font-size: $h1-size;
}
h2 {
  @include dropshadow(darkblue);
  font-size: $h2-size;
}
```

CSS output:  
```css  
h1 {
  color: black;
  text-shadow: 2px 4px #666666;
  font-size: 3.6em; }
h2 {
  color: darkblue;
  text-shadow: 2px 4px #5858ff;
  font-size: 2.4em; }
```

### Clear fix mix-in  
A very common problem is to define a section of your page with elements that are based upon floats. You have to “clear” your floats before you begin the next section, or else the browser will cram the next bit up against the last float. The most common method in use today uses the pseudo-elements `:before` and `:after` to handle the clear, avoiding the need to create extra markup. Often a `.clearfix` class is used on elements, but here we’re going to build it in via a mix-in.

Start with SCSS:    
```scss
@mixin clearfix {
  &:before, &:after {
    content: " ";
    display: table;
  }
  &:after {
    clear: both;
  }
}
```  

Use in SCSS:  
```scss  
.row {
  @include clearfix;
  margin-left: 10px;
  margin-right: 10px;
}
.row > .box {
  float: left;
  padding: 10px;
}
```

Compiled CSS:  
```css  
.row {
  margin-left: 10px;
  margin-right: 10px;
}
.row:before, .row:after {
  content: " ";
  display: table;
}
.row:after {
  clear: both;
}
.row > .box {
  float: left;
  padding: 10px;
}
```

## Math operations
With CSS you have to be explicit about everything, including numbers.
With Sass, you can write math to calculate numbers for you:
* [Addition](http://sass-lang.com/docs/yardoc/file.SASS_REFERENCE.html#number_operations)  
* [Subtraction](http://sass-lang.com/docs/yardoc/file.SASS_REFERENCE.html#number_operations)  
* [Multiplication](http://sass-lang.com/docs/yardoc/file.SASS_REFERENCE.html#number_operations)  
* [Division](http://sass-lang.com/docs/yardoc/file.SASS_REFERENCE.html#division-and-slash) [division is special, check the documentation link for why and how]  

Sass input:    
```scss
$layoutWidth: 960px;
$defaultPadding: 16px;
#sidebar {
  width: $layoutWidth/3;
  float: left;
}
#main {
  padding: $defaultPadding;
  width: ($layoutWidth/3)*2 - $defaultPadding*2;
  float: right;
  &:after {
    content: '';
    clear: both;
  }
}
```

CSS output:  
```css
#sidebar {
  width: 320px;
  float: left; }
#main {
  padding: 16px;
  width: 608px;
  float: right; }
#main:after {
  content: '';
  clear: both; }
```

## Color Functions
Color manipulation functions are built in to Sass. This is great for putting together accent colors based on a brand.
* darken – darkens a color  
`darken($color, $amount)`  
* lighten – lightens a color  
`lighten($color, $amount)`  
* opacify – makes a color more opaque  
`opacify($color, $amount)`  
* transparentize – makes a color more transparent  
`transparentize($color, $amount)`  

Sass input:    
```scss  
$background: #f3f3f3;
$text_color: darken($background, 30%);
$accent_color: lighten($text_color, 10);
body {
  color: $text_color;
  background: $background;
  a {
    color: $accent_color;
  }
}
```  

CSS output:  
```css  
body {
  color: #a7a7a7;
  background: #f3f3f3; }
body a {
  color: silver; }
```

## Comments
Sass allows both multi-line and single-line comments. Multi-line comments are passed through to the compiled CSS. Single-line comments are not passed through. This is useful for hiding development notes from the end site.  

```scss
/* Multi-line comments
 * are passed through
 */
// single line comments are not
$layoutWidth: 960px;

body {
  width: $layoutWidth;
}
```

## Looping  
Sass gives you the ability to run in loops to build up CSS classes. Sass provides three types of loops:  

```scss  
@for
@each
@while
```

### For Looping  
Much like JavaScript’s for, `@for` runs over a range:  

Sass input:  
```scss  
@for $i from 1 through 3 {
  .item-#{$i} { width: 2em * $i; }
}
```  

CSS output:  
```scss  
.item-1 {
  width: 2em;
}
.item-2 {
  width: 4em;
}
.item-3 {
  width: 6em;
}
```

### Each Looping  
More like a mapping function, `@each` lets you run through several values:  

Sass input:  
```scss  
@each $animal in puma, sea-slug, egret {
  .#{$animal}-icon {
    background-image: url('/images/#{$animal}.png');
  }
}
```

CSS output:  
```css  
.puma-icon {
  background-image: url("/images/puma.png");
}
.sea-slug-icon {
  background-image: url("/images/sea-slug.png");
}
.egret-icon {
  background-image: url("/images/egret.png");
}
```

### While Looping  
The `@while` loops keeps running as long as it’s condition is true, like so:  

Sass input:  
```scss  
$i: 6;
@while $i > 0 {
  .item-#{$i} { width: 2em * $i; }
  $i: $i - 2;
}
```  
CSS output:  
```css  
.item-6 {
  width: 12em;
}
.item-4 {
  width: 8em;
}
.item-2 {
  width: 4em;
}
```

## Branching  
Along with looping, Sass provides a way to branch based on the evaluation of an expression using:  
* `@if`  
* `@else`  
* `@else if`  

Sass input:   
```scss  
$type: monster;
p {
  @if $type == ocean {
    color: blue;
  } @else if $type == matador {
    color: red;
  } @else if $type == monster {
    color: green;
  } @else {
    color: black;
  }
}
```  

CSS output:  
```css  
p {
  color: green;
}
```

## Organizing  
Use the **ITCSS - Inverted Triangle CSS** where we try to perform **Low Specificity and High Genericity** down to **High Specificity and Low Genericity**.

For example, use the following for reference:  
* Settings  
* Tools  
* Generic  
* Base  
* Objects  
* Components  
* Overrides  

### Settings  
This is where your variables go, and is a good place to load web fonts, too!  

For example:  
```scss  
$body-bg: lightgreen;
$accent-bg: darken($body-bg, 40%);

@import 'https://fonts.googleapis.com/css?family=Open+Sans';
$font-stack: 'Open Sans', sans-serif;
```  

### Tools  
The home of mixins and functions.  

For example:  
```scss
@mixin clearfix {
  &:before, &:after {
    content: " ";
    display: table;
  }
  &:after {
    clear: both;
  }
}
```
### Generic  
Style attributes to apply to everything on the page.  

For example:  
```scss
* {
  -webkit-box-sizing: box-content;
  -moz-box-sizing: box-content;
  -ms-box-sizing: box-content;
  -o-box-sizing: box-content;
  box-sizing: box-content;
}
```  

### Base (Resets)   
Bare element style attributes. This is where you do your resets and element defaults.  

For example:  
```scss  
a {
  text-decoration: none;
  &:hover {
    @include glow($link-hover-color);
  }
}
```  

### Objects   
From this point onward, everything is class based. This is where you address major page objects, such as the page header, main content, and so on.  

For example:  
```scss  
.page-header {
  h1 {
    font-family: $header-font-stack;
  }
}
```

### Components  
Components refer to UI components, such as menu items, icons, etc. Generally things that might appear in several places on a page.    

For example:  
```scss  
.jump {
  @include iconFont;
  color: $jumpColor;
  &.up { left: $jumpOffset; }
  &.down { right: $jumpOffset; }
  &:hover { color: $jumpHoverColor; }
}
```  

### Overrides  
Page overrides. These should be kept to a bare minimum. These things are known as “The Hall of Shame”. Consider using a targeted class in the Components section instead.   

For example:  
```scss  
// i demand this be in red!
header nav ul li:last-child a {
  color: red !important;
}
```
