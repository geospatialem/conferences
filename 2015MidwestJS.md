# MidwestJS 2015 (Minneapolis, Minn.)

<img src="https://cloud.githubusercontent.com/assets/5023024/9292291/eb7ceff0-43b4-11e5-879d-91f54cc6c33c.png" width="25" height="25">  [Midwest JS](http://www.midwestjs.com) is a premier technology conference focused on the JavaScript ecosystem. There were a variety of talks from well­known speakers in the community in a typical presentation format. 

**Session Tracks:**
* *Beginner Track*: JavaScript fundamentals, jQuery, jQuery UI, etc.
* *Frameworks Track*: Angular.js, Knockout.js, Ember.js, Backbone.js, etc.
* *Node Track*: Aything based on Node.js
* *Mobile­Track*: PhoneGap, Appcelerator, etc.
* *Testing Track*: TDD, Jasmine, etc.
* *Miscellaneous Track*: Anything that doesn't fit into the others

**Sessions:**  
* *[Opening Keynote: The Art of Simplicity](#keynote-the-art-of-simplicity-venkat-subramaniam)*, Venkat Subramaniam  
* *[Writing Better jQuery Infused JavaScript](#writing-better-jquery-infused-javascript-ken-dale--slides)*, Ken Dale  
* *[Components are the Future of the Web: It's Going to be Okay](#components-are-the-future-of-the-web-its-going-to-be-okay-tessa-thornton)*, Tessa Thornton  
* *[Better Debugging in Chrome](#better-debugging-in-chrome-josh-longanecker)*, Josh Longanecker  
* *[Developing for Firefox OS: It's just the Web... or is it?](#developing-for-firefox-os-its-just-the-web-or-is-it-dan-callahan)*, Dan Callahan  
* *[That's so Prototypical](#thats-so-prototypical-jordan-kasper)*, Jordan Kasper  
* *[Enterprise JavaScript Apps with TypeScript](#enterprise-javascript-apps-with-typescript-kurt-wiersma-slides)*, Kurt Wiersma  
* *[JavaScript Forensics](#javascript-forensics-todd-gardner-slides)*, Todd Gardner  
* *[Test Them Puzzles: What Test-Driven Learning Can Teach About JS and TDD](#test-them-puzzles-what-test-driven-learning-can-teach-about-js-and-tdd-branden-byers-slides)*, Branden Byers  
* *[Edge of Tomorrow: Introducing Microsoft's New Browser](#edge-of-tomorrow-introducing-microsofts-new-browser-david-giard-slides)*, David Giard  
* *[Adventures in Test-Driven Development](#adventures-in-test-driven-development-jeremy-lund)*, Jeremy Lund  
* *[Closing Keynote: The Current State of JavaScript](#keynote-the-current-state-of-javascript-jon-dejong)*, Jon DeJong  


## Thursday, August 13th, 2015
### Keynote: The Art of Simplicity ([Venkat Subramaniam](http://www.twitter.com/venkat_s))
* “Life is really simple, but we insist on making it complicated.” ― Confucius 
* “Any intelligent fool can make things bigger, more complex, and more violent. It takes a touch of genius, and a lot of courage, to move in the opposite direction.” ― Albert Einstein
* “I conclude there are two ways of constructing software design: one way is to make it so simple there are obviously no deficiencies, and the other way is to make it so complicated that there are no obvious deficiencies.” ― Tony Hoare
* “A designer knows he has achieved perfection not when there is nothing left to add, but when there is nothing left to take away.” ― Antoine de Saint-Exupery
* “You can recognize truth by its beauty and simplicity. When you get it right, it is obvious that it is right, at least if you have any experience, because usually what happens is that more comes out than goes in.” ― Richard Feynman  
* “Everything should be made as simple as possible, but not simpler.” ― Albert Einstein
* “Simplicity is the ultimate sophistication.” ― Leonardo da Vinci
* We love to say we are working on monsters, and not working on solving simple solutions. We feel good when we make things complex.  
* It's difficult for us to focus on simplicity because we react on our behavior and emotions.
* It's hard to know what is simple, so we can instead focus on what is not simple. 

So let's focus on what is not simple:  

1.**Simple's not clever**: It is a realization, a *clear solution!!* How do we manage code when there is no logic? Would you do this to your children, name them ```p```? We lose abstraction of our ideas.  

2.**Simple's not necessarily familiar**: *(aka accidential complexitivity)* Something may be complex for a minute. Familiarity can look, or even be complex, it's all about understanding. 

![](https://cloud.githubusercontent.com/assets/5023024/9292098/17d42a32-43ab-11e5-84c2-4ba12481f918.JPG)

One hard realization is the *self-inflicting wound pattern*, when we forget to do something one day, and it continues to build up over time. Focus on: *what* you are doing, don't confuse, and use *declarative* code (it's simpler)! See: [Venkat's blog post](http://blog.agiledeveloper.com/2015/08/prefer-functional-style-over-imperative.html) for an example of functional vs. imperative code. Simple has fewer moving parts, illuminate them!       

3.**Simple's not over-engineered**: See: *the automated back scratcher comic strip* below. For example: A phone call with someone in the room vs. an in-person discussion).    

![](https://cloud.githubusercontent.com/assets/5023024/9292409/e0384650-43bc-11e5-912a-4b09bb3b4fdb.jpg)  

![](https://cloud.githubusercontent.com/assets/5023024/9292094/e7eb7ed8-43aa-11e5-9d3e-d178b25ecb4a.JPG)  

4.**Simple's not terse**: Don't confuse simple/concise with terse. It's about extensibility. Terse vs. concise: *Terse* is short, and waiting to hurt you when you least expect it.

![](https://cloud.githubusercontent.com/assets/5023024/9292103/69e01c14-43ab-11e5-9bb0-9439c3d40a24.JPG)

*Concise* is transparent. If you don't know why your application in production is failing every three weeks, find out why and break down the steps. 

5.**Simple keeps you focused**: Focus keeps down the distractions. (e.g. Search Engines: Yahoo has news distractions, *why did we come here again?*, Bing is beautiful, *do we really want to search and lose this beautiful picture?*, and Google is simplistic, we don't get lost in anything, *let's start our search*). This is extremely hard to do, to do something simple. It is *extremely valuable* to value someone else's time. Focus on the user, and don't distract them. This takes *genius* and *courage*.  

![](https://cloud.githubusercontent.com/assets/5023024/9292115/0d1da360-43ac-11e5-949a-63f073a49f55.JPG)

6.**Simple fails less**: (e.g. Manhole's shape is a circle, one size fits all)!  

7.**Simple's easy to understand**: Simple is easy to work with!  

8.**Simple is elegant**: Fluancy., or code that doesn't look like a tornado! When there is nothing to take the focus away from something, it is truly elegant (e.g. Mona Lisa painting). This presents the *Architect's dilemna* (e.g. Trinity Church and an adjacent building in Boston, Mass' reflection off the church).  

9.**Simplicity has to evolve**: We have all said, *my code simply sucks* at some point. Over time, things change, and as we change, simplicity will as well. Simple makes things easy, but its certainly not easy.  

**Resources:**  
* [Structure and Interpretation of Computer Programs](http://www.amazon.com/Structure-Interpretation-Computer-Programs-Engineering/dp/0262510871), book

### Writing Better jQuery Infused JavaScript ([Ken Dale](http://www.twitter.com/kendaleiv)),  [Slides](http://kendaleiv.com/jquery-js-refactor/#/)  

**Keys for Maintainability/Testability/Warm Fuzzies:**  
* **External files** (Good practice): Caching JavaScript in-browser.  
* **Strict mode** Helps with troubleshooting.  
```javascript  
function () {
  'use strict';

  // Code here
};
```  
* **Wrap in Life**: Function wrapped in params ```(``` and ```)```. This *thing* will immediately execute as it is an immediately-invoked function expression, which helps scope variables and prevent unintended sharing between components. This will shield the library from tampering (which is useful with global variables). Good resource [Atom editor](https://atom.io) (Windows/Apple).  
```javascript
(function () {
  'use strict';

  // Code here
})();
```  
* Use the **Shorthand, Luke**: Using document.ready, changing ```click``` → ```on```, changing ```success``` → ```done``` (JavaScript process/chaining). Avoid deprecated items, like ```jQuery.live()``` (see jQuery [docs](https://api.jquery.com/category/deprecated)).  
~~```$(document).ready(function () { /* Code here */ });```~~  
```$(function () { /* Code here */ });```  

**jQuery items:**  
Use ```on``` rather than ```click```. For example:  
~~```$('#fetch').click(function () { /* Code here */ });```~~  
```$('#fetch').on('click', function () { /* Code here */ });```  

Use ```done``` rather than ```$.ajax options success```. For example:    

~~```$.ajax({ success: function (res) { /* Code here */ } });```~~  
```$.ajax().done(function (res) { /* Code here */ });```  

**Other Notes:**
* “If you're having a problem up front, thats normal.”
* **Refactoring**: AJAX provides data and is a ```promise``` in itself.  
* **Testing**: e.g. Jasmine for Frameworks/Libraries. Test descriptions with ```it``` using ```expect``` and ```toBe``` statements. There are custom Jasmine matches, such as ```spyOn``` (see [documentation](http://jasmine.github.io)).  
* “**DRY** test your code (aka **D**on't **R**epeat **Y**ourself). The opposite of DRY testing is **WET** (aka **W**e **E**njoy **T**yping).” Ideally have one single representation in your code base.
* **Other ways:** requireJS, ES6 modules (which may be the future), etc.
* **Start**: 44 lines of code. **End:** HTML: 25 lines, JS: 127 lines. *Sometimes simplicity requires more lines of code*, for troubleshooting and for helping ourselves in the future. Used the Jasmine HTML runner.

**Resources:** 
The project [code](http://www.github.com/kendaleiv/jquery-js-refactor), reference individual commits to see the refactoring process from start → finish.

### Components are the Future of the Web: It's Going to be Okay ([Tessa Thornton](http://www.twitter.com/tessthornton))  

* HTML is semantic (clean and virtuous)
* We haven't kept up on complex UI's
* HTML is not just for content (e.g. adding in JSON files from JavaScript into HTML). HTML isn't just for content, and it never was.
* **Imperative**: the steps to achieve a desired result *versus* **Declarative**: the desired result, leaves the implementation up to something else (e.g. SQL).
* HTML has declarative API's, or a contract of inputs + outputs. HTML needs to know what to put in it, which is especially true in HTML5.
* “We're writing JavaScript like we don't have any control over HTML.” 
* In 2009, AngularJS was created with the idea of seperating HTML from the DOM, the *seperation of concerns*. Not just one implementation. We can make our own delcarative **attributes** and **elements**.
* The future will focus content with HTML and action with JavaScript, specific actions wired together to focus on your application.
* “You're going to *pollute* your HTML and you're going to like it!”

**Dogma:**  
* **HTML**: Content  
* **JavaScript**: Behavior  
* **CSS**: Presentation  

**Web Components** (see: *tab example*):  
1. Custom elements  
2. Shadow DOM  
3. Templates  
4. HTML imports  

**Benefits (+):**  
* Reusability  
* Meaningful HTML  
* Encapsulation  
* Composability  
* Philosphy has spread to frameworks  
* Browsers are already doing it themselves  

**Cons (-):**
* Browser specifications aren't great (*yet*). 
* Sometimes needs some tweaks.  

**Options:**  
1. **[Polymer](http://www.polyer-project.org)**  
2. **[AngularJS](https://angularjs.org)** directives, framework  
3. **[EmberJS](http://emberjs.com)** components, framework  
4. **[ReactJS](http://facebook.github.io/react)** components, framework: A much different look at components.  
5. **[Twine.js](https://bitbucket.org/klembot/twinejs)**, library: Declarative data-binding library.  
6. **[Knockout.js](http://knockoutjs.com)**, library: Declarative data-binding library.  
7. Native browser support (*coming soon*)  

**Resources:**
* [Our Best Practices are Killing Us](http://www.slideshare.net/stubbornella/our-best-practices-are-killing-us), Nicole Sullivan
* Demo utilized [VanilaJS](http://vanilla-js.com) from scratch, and [Polymer](https://www.polymer-project.org) since it is less opinioned.

### Better Debugging in Chrome (Josh Longanecker)

**Tricks + Tips**:  
* **Scroll into view** from code → browser.  
![chromescrollintoview](https://cloud.githubusercontent.com/assets/5023024/9294486/2ab4f3b6-4414-11e5-976e-73279b834b32.png)  
* **Awaits** tab: Will showcase the performance on your code.  
* **Pretty Print**: under ```Sources``` → ```{ }``` in the lower-left corner of the window.  
![chromeprettyprint](https://cloud.githubusercontent.com/assets/5023024/9294179/3736dfb8-440b-11e5-9b70-e23e13a05386.png)  
![chromeprettyprint2](https://cloud.githubusercontent.com/assets/5023024/9294188/593f4d0c-440b-11e5-9891-7614e57cb9d4.png)  
  
* **Breakpoints**: Conditional breakpoints, lists breakpoints to turn on/off in the right-hand window, step over breakpoints.
* **Blackbox script**: The debugger will ignore scripts. To enable right-click the JavaScript file → ```Blackbox script```.  
![chromeblacboxscript](https://cloud.githubusercontent.com/assets/5023024/9294519/23e44630-4415-11e5-91bf-0d01da063757.png)

* **Console.log(); messages**: ```console.error();```, ```console.log();```, ```console.group();```, ```console.groupEnd();```, ```console.groupLog();```, ```console.groupCollapsed();```, ```console.assert();```, etc.
* **Preserve log**: Good practice when testing out AJAX calls (Before/After)
* **Timeline**: ```console.time();``` and ```console.timeEnd();```.

**Resources:**  
* [Chrome documentation](https://developer.chrome.com/devtools)  

### Developing for Firefox OS: It's just the Web... or is it? ([Dan Callahan](http://www.twitter.com/callahad))  
Mozilla is working with smartphones and tv's solely using web development.

**Resources:**  
* [Mozilla Developer Network](https://developer.mozilla.org/en-US)
* [Firefox Developers](http://www.firefox.com/developer): Add instance developer *(currently in Beta)*

### That's so Prototypical ([Jordan Kasper](http://www.twitter.com/jakerella))

* JavaScript isn't really object-oriented (*under the covers*).
* JavaScript is a multi-paradigm language.
* Even functions are objects (e.g. methods, properties, and null objects).
* **Chain of objects** (e.g. [Python DunderAlias](https://wiki.python.org/moin/DunderAlias)).

```javascript 
//Functional JavaScript
function addTo (x, y) {
  return x + y;
}
```

```javascript
//Non-Functional JavaScript
var x = 1;
function addTo(y) {
  return x + y;
}
```

**New Keyword:**
* Not needed, if it isn't a class.
* Is three action: 1. **Empty Object**, 2. **Objects property prototype**, and 3. **Constructor method** (Note: The following is needed for support in IE 8/9, ```object.create shim```).

**Inheritence:**
* Property: 
```javascript
for (variable in object) {
    code to be executed
} 
```
* Method
```javascript
function person(firstName, lastName, age, eyeColor) {
    this.firstName = firstName;  
    this.lastName = lastName;
    this.age = age;
    this.eyeColor = eyeColor;
    this.changeName = function (name) {
        this.lastName = name;
    }
}
```

## Friday, August 14th, 2015
### Enterprise JavaScript Apps with TypeScript ([Kurt Wiersma](http://www.twitter.com/kwiersma)), [Slides](https://github.com/midwestjs/2015/blob/master/enterprise-javascript-apps-with-typescript/Using%20TypeScript%20To%20Build%20Better%20Apps.pdf)

* **JavaScript is a valid typescript**
* “It takes discipline to write good code.”
* TypeScript is following ECMA Script 6.
* Types are optional.
* TypeScript doesn't force you to use classes or interfaces.
* Create custom [definitions](http://definitelytyped.org/tsd) easily (e.g. ```pusher.d.ts```). Reference by *pulling down*.
* Existing JavaScript libraries were built using TypeScript (e.g. [DefinitelyTyped](http://definitelytyped.org), jQuery, Angular, Ember, Backbone).
* **Refactoring! Tooling!**

**TypeScript**:
* Open-sourced by Microsoft (the first Microsoft product to do so).  
* Superscript of JavaScript (on top of the JavaScript syntax).  
* Compiles to JavaScript.  
* Works with any browser, host, and operating system (OS).  
* JavaScript is a valid TypeScript.  
![](https://cloud.githubusercontent.com/assets/5023024/9292273/307603c2-43b4-11e5-9fa5-ab6440fc72cd.png)  

**Features**:
* Classes
* Modules
* Interfaces (optional)
* Genertics
* Arrow functions
* References
* Type definitions
* Better ```this``` usage, *by default*

**Pros**:
* Syntax is JavaScript and type info
* Targets ES6
* Optional types
* Classes, generics, and interfaces (object oriented)
* Fixes ```this```

**Cons**:
* Compile step
* Debugging (use source maps)
* Another language / tool to learn

**Enterprise (Defined)**:
* > 2 developers on a team/project.
* Mix of junior developers.
* Large code bases (which gives the ability to refactor code).
* Leverage existing code from other teams/companies (e.g. Type definition file, such as C/Java).
* Proven technology (*stable*), not necessarily bleeding edge, but cutting edge.
* Productive, to produce better code.

**Why Use Types?**:
* Create structure for large code bases/teams.
* Catch errors early.
* ***Provide a structured API*** (documentation from chaos).
* Tooling can provide better code completion and refactoring.

**Getting Started**:  
TypeScript compiles library files. Creates a Grunt/Gulp task that will manage/build.

Support includes the following IDE's at no charge: Eclipse (*plugin*) and Visual Studio Core. It also includes the Atom editor at no cost, and Sublime for a small cost.
```javascript
npm -g typescript
tsc --sourcemap --out js/Application.js js/_all.ts
```

**Making a Better Application**:
* Gradually move JavaScript to TypeScript.
* Add types, a better way to structure code along the way.
* Can make working with an API easier to learn.

**Resources**:
* [Angular in 20 minutes](https://github.com/DanWahlin/AngularIn20TypeScript)
* Expense Manager (*link coming soon*)

### JavaScript Forensics ([Todd Gardner](http://www.twitter.com/toddhgardner)), [Slides](https://speakerdeck.com/toddhgardner/javascript-forensics)

* “JavaScript inevitably breaks for everyone.”  
* “There's a lot of broken JavaScript on the internet.” In fact, on average there is a [40% failure rate](https://trackjs.com/blog/the-state-of-client-side-javascript-errors).  
![](https://cloud.githubusercontent.com/assets/5023024/9292125/df164e30-43ac-11e5-8025-7ab7c1199d63.gif)  
* “JavaScript on the web is still the Wild West.”  
* It relates a few things. In particular: shipping out software to a treacherous landscape of: a few browsers (Chrome, Safari, Internet Explorer, Firefox, Opera, etc.), several third-party scripts, lots of application frameworks, and an army of JavaScript libraries.
* “Error messages get gnarly.” 

**Most Common JavaScript Outlaws**:  
1. Script error  
2. 3rd-party error  
3. Context error  
4. Data error  
5. Loading error  
6. Memory error  

**_1. Script error_**:  
* **Impact**: Unknown, but frequent and all browsers are affected (e.g. 2,481 errors). 
* **Place of Origin**: Browser obfuscation.  
* **Characteristics**: Noisy  
* **Associates**: 3rd party scripts and CDN's.  
* **Remarks**: Conceals other errors. Apprehend with CORS and crossorigin attributes.  

*Console error log recording:*  
```javascript
window.onError = function () {
  console.error("Recorded: ", arguments);
}
```

*Chrome headers:*  
Open the ```Network``` tab → Reload the application → Click the file in question → Select the ```Headers``` tab.  
![chromeheaders](https://cloud.githubusercontent.com/assets/5023024/9294217/5163f3b6-440c-11e5-9bc4-a64002f2bb28.png)  

*Add a cross-orgin of anonymous to the file:*  
If you add ```crossorgin="anonymous"``` and the response the JavaScript file was loaded from sends an ```Access-Control-Allow-Origin: *``` you get noted about the real error message and the line of the file and the column the error accrues. If you add ```crossorgin="anonymous"``` and the response doesn't contain ```Access-Control-Allow-Origin: *``` the browser will block the script (e.g. ```<script crossorigin="anonymous" src="url"></script>```).  

**_2. 3rd party error_**:  
* **Impact**: Global (e.g. error rate of 15.4/hour, error change is up 523%).
* **Place of Origin**: Uncontrolled changes.  
* **Characteristics**: ```getRandomAds``` is not defined. Sudden bursts of violence.  
* **Associates**: SaaS, Analytics, CDN.  
* **Remarks**: External hosted scripts are beyond our control. Performance comes with risk (e.g. a typo).  

**_3. Context error_**:  
* **Impact**: Major  
* **Place of Origin**: Functional arguments.  
* **Characteristics**: Cannot read property ```destroy``` of undefined (not defined).  
* **Associates**: Callbacks, promises.  
* **Remarks**: Usually can be discovered through a test.  

*Problem is a result of*:  
User Click:  
```html
<button class="js-delete-statement">
```  
Error:  
```javascript
Cannot read property 'destroy' of undefined.  
```  

**Potential Resolutions**:  
* Source maps → Minified files (Chrome developer tools → Sources → select JavaScript file → click the ```{}``` (Pretty Print) button in the lower left corner.  
![chromeprettyprint](https://cloud.githubusercontent.com/assets/5023024/9294179/3736dfb8-440b-11e5-9b70-e23e13a05386.png)  
![chromeprettyprint2](https://cloud.githubusercontent.com/assets/5023024/9294188/593f4d0c-440b-11e5-9891-7614e57cb9d4.png)  
* Chrome developer tools → Sources → Right-hand menu *Call stack* → ☑ *Async*  
![chromeasync](https://cloud.githubusercontent.com/assets/5023024/9294193/74a02526-440b-11e5-9eba-e92a3e5af071.png)  

**_4. Data error_**:  
* **Impact**: Isolated  (e.g. 1 user affected, 2,124 errors)  
* **Place of Origin**: API contract changes.  
* **Characteristics**: ```a.text.substr``` is not a function, as a result of production faults.  
* **Associates**: Separate teams, third parties.  
* **Remarks**: Difficult to test for every possibility. Weigh risk for your application.  

*Troubleshooting*:
* Chrome Developer tools → Network → XHR (XmlHttpRequest). XHR allows you to debug AJAX requests. You can add a breakpoint by going to the "Sources" tab and selecting "XHR Breakpoints".  
![](https://cloud.githubusercontent.com/assets/5023024/9292161/7a174fb4-43ae-11e5-9a58-db9b5a06113c.png)  
* The issue in this instance was related to a text vs. number when the code expects text.  

**_5. Loading error_**:  
* **Impact**: Major (e.g. 129 users affected, 134 errors seen).  
* **Place of Origin**: Coverage ghettos, elevators (aka areas with little/no/spotty service).  
* **Characteristics**: ```INLINE_ADS``` is not a function, ```X``` is undefined.  
* **Associates**: Mobile.  
* **Remarks**: Verify and fallback load scripts. Async and AJAX can help detect.  

*Notes*:
* Sometimes ```<script>``` tags fail, even just one. If it fails, will your application load? 
* Mobile devices with DNS lookout for CDN's fail.  

**_6. Memory error_**:  
* **Impact**: Catastrophic (currently only identified through e-mails complaints, phone calls, tweets, in-person complaints, etc. as there is no way to monitor this behavior since the browser crashes. Similar to the *blue screen of death* seen in the Windows operation system).  
* **Place of Origin**: Detached elements.  
* **Characteristics**: Crashing browser, GB tabs.  
* **Associates**: Events on detached DOM. 
* **Remarks**: Periodic checks for kidnapping. Named functions assist in apprehension.  

*Troubleshooting*:  
* Chrome Developer tools → Network → All. Zoom in on particular requests and/or modify the timeline to determine the method requests (check out the *preview*, *response*, and *timing* tabs as well).
* Under the Chrome Developer tools → Network → *Record* button, to see the requests over specific actions on the page for additional troubleshooting.  
* After running a recording session, check out the memory graphs (check the ☑ *Memory* checkbox) in the *Timeline* tab to view the: Used JS Heap, Documents, Nodes, Listeners. Zoom to the main thread (that gives location in the graph).  
![chrometimeline](https://cloud.githubusercontent.com/assets/5023024/9294213/2823f21c-440c-11e5-9412-2aeb1e6859f8.png)  
* Detach elements →  Drop when gone from the page.  


### Test Them Puzzles: What Test-Driven Learning Can Teach About JS and TDD ([Branden Byers](http://www.twitter.com/brandenbyers)), [Slides](http://brandenbyers.com/slides/test-them-puzzles)

* “**Learning to code is hard,** puzzles are a great way to make it fun.”  
* We need that **Aha! Dopamine drip moment**, they are important! “The more we do it and achieve these moments the more exciting and rewarding it gets!”  
* An hour is a good time for digesting a puzzle. If you can't solve it, put it off to the side and try again. When you do solve it, you'll get that Aha! moment, see any hurdles from the past, and/or question why it was a harder problem before.  
*  Puzzles are nimble.
*  It's hard to describe in a simple way (see: the *Puzzle Example ― Ryming Numbers Poem* below).
*  I don't know how to solve it, but I can think about the problem and how to approach it.  
*  “Think of things in **bite-size chunks**.”  
*  Syntactic Wilderness: Wander and you might get lost.   
*  “Think of the test as the end-product itself.”  
*  For testing, uses [ChaiJS](http://chaijs.com)'s ```expect()```, ```should()```, and ```assert()```. For example:  
```javascript
  expect('something').to.contain('thing');
  expect('Hello World').to.be.a('string');
```
* Contribute (e.g. [Code Camp Github Repo](https://github.com/FreeCodeCamp/FreeCodeCamp), and [Code Wars](http://codewars.com/kata/search/javascript?q=))!

**Programmer Practice**:
* Athletes train
* Musicians rehearse
* Lawyers and doctors practice

**Do you Code like a Parrot or a Crow?**:  
**Parrots**:  
![parrot](https://cloud.githubusercontent.com/assets/5023024/9294395/c5897612-4411-11e5-9bd2-5ff56e9f017d.jpg)  
* Inquisitive  
* Destructive exploration  
* Playful learners  
* Pull, tear, scratch, probe  
* Haphazardly dig for food  

**Crows**:  
![crow](https://cloud.githubusercontent.com/assets/5023024/9294396/c7aef106-4411-11e5-91ac-6a87f3bb850d.jpg)  
* Curious  
* Explore from a distance  
* Methodical learners  
* Graceful tool users  
* Precisely prod for food  

**Puzzle Samples**:  
Assumptions === Bad! For example:  
```javascript
var add = function (a, b) {
  return a + b;
};

expect(add(2, 2).to.equal(4));

expect(add(2, '2').to.equal('22'));

expect(add('con','cat').to.equal('concat'));
```
Instead use:  
```javascript
var add = function (a, b) {
  if(typeof a + b === 'string') {
    return 'Go fish';
  }
  ...
};

expect(add('con','cat')).to.equal('Go fish');
expect(add(2, 2)).to.be.a('number')
```

```javascript
var add = function (a, b) {
  return parseInt(a) + parseInt(b);
};

expect(add(2, '2').to.equal(4));
expect(add(2.22, 2.22).to.equal(4.44));

// AssertionError: expected 4 to equal 4.44
```

**Puzzle Example ― Slasher Film**:  
Return the surviving elements of an array after chopping off n elements from the head (e.g. ```slasher([1, 2, 3], 2);```).  

```javascript
expect(slasher([1,2,3],2)).to.equal([3]);
expect(slasher([1,2,3],0)).to.equal([1,2,3]);
expect(slasher([1,2,3],9)).to.equal([]);

expect(slasher([1,2,3],2)).to.equal(['Three, you're lucky to still be.']);
expect(slasher([1,2,3],0)).to.equal(['All numbers live another day.']);
expect(slasher([1,2,3],9)).to.equal(['It is a sad day.']);

expect(slasher(['1,354','22','4900'],1)).to.equal(['Four thousand nine hundred and twenty-two; you are amongst the lucky few.']);
```  
**Solution**: Return a string of the *English word equivalents* of the surviving elements *(numbers)* in an array after chopping off n elements from the head. The numbers must be listed from last to first. The string should be finished with a phrase that rhymes with the last number listed.  

**Puzzle Example ― Ryming Numbers Poem**:  
You will be given an array of numbers. Each number will be between 0 and 9. These numbers may be integers or strings. If a number is in a string, it may be a digit or word. Return a nonsense poem, where each line starts with a number from the array followed by a phrase ending in a word that rhymes with that number.  

*Nine, you smell like wine  
Five, chicken dumplings make me feel alive  
Three, you be lost deep in the sea  
Two, please stop sniffing glue  
One, this poem is done*  

```javascript
var rhymingNumberPoem = function(arr) {
  // this is a poet but didn't know it
  return str;
};

var shortArr = [9,5,3,1];
var longArr  = [9,5,3,1,5,4,3,5,6,3,2,3,4,7,5,2,3,4,7,10,23,4,2];

describe('Rhyming Number Poem', function() {
  it('should return a string', function() {
    expect(rhymingNumberPoem(shortArr)).to.be.a('string');
  });
  it('should return correct number of lines from short array', function() {
    expect(rhymingNumberPoem(shortArr).split('\n').length).to.equal(shortArr.length);
  });
  it('should create a short rhyming poem', function() {
    expect(rhymeChecker(rhymingNumberPoem(shortArr))).to.equal(true);
  });
  it('should create a long rhyming poem', function() {
    expect(rhymeChecker(rhymingNumberPoem(longArr))).to.equal(true);
  });
});

var rhymeChecker = function(str) {
  var arr = str.split(/,|\./).join('').split("\n");
  if(str.length < 1 || arr[0].split(' ').length < 3) {
    return false;
  }
  var count = arr.reduce(function(a, b) {
    var words = b.split(' '),
        firstWord = words[0].toLowerCase(),
        lastWord = words[words.length - 1].toLowerCase();
    if(numberRhymes[firstWord].match(lastWord)) {
      return a + 1;
    }
    return a;
  }, 0);
  if(count < arr.length) {
    return false;
  }
  return true;
};

  zero: 'hero giro tiro nonzero subzero',
  one: 'won done run son none sun gun fun tion ton nun shun sion bun donne dun fon pun rien bn cen gon hun jun tonne tun ven yean naan spun fron seisin stun toucan anyone begun undone outdone outrun spline rerun redone everyone overrun overdone cretonne misdone twentyone'
```

**Write Kickass Puzzles**:
* Write Descriptions
* Generate tests
* Double/Triple/Quadruple check your cases.
* Solve, then bathe in Dopamine!
* Share/Repeat!

**Code Challenge Websites**:  
* **[Code Wars](http://codewars.com)**  
* **[Free Code Camp](http://freecodecamp.com)**  
* [Hacker Rank](http://hackerrank.com)  
* [Coder Byte](http://coderbyte.com)  
* [Project Euler](http://projecteuler.net)  
* [Node School](http://nodeschool.io)  
* [Exercism.io](http://exercism.io)  

**Resources**:  
* [Archimedes' Puzzle: Ostomachion](https://en.wikipedia.org/wiki/Ostomachion), solve the unique ways to reorganize the shapes into a box without rotating any of the objects.    
![ostomachion](https://cloud.githubusercontent.com/assets/5023024/9294382/123ac048-4411-11e5-8f3f-a0b307cd1093.png)  
* [Rosetta Code: Towers of Hanoi](http://rosettacode.org/wiki/towers_of_hanoi) 
  ![tower_of_hanoi](https://cloud.githubusercontent.com/assets/5023024/9294412/3537fa4c-4412-11e5-89f3-47843e154df6.jpeg)  
* [Flexibility in Problem Solving and Tool Use of Kea and New Caledonian Crows in a Multi Access Box Paradigm](http://journals.plos.org/plosone/article?id=10.1371/journal.pone.0020231), article (Parrots and crows)  

### Edge of Tomorrow: Introducing Microsoft's New Browser ([David Giard](http://www.twitter.com/davidgiard)), [Slides](https://onedrive.live.com/view.aspx?resid=7048EC40C0AC24C1!773074&ithint=file%2cpptx&app=PowerPoint&authkey=!AGhhQF1Vn656zrQ)

* Evolving world of computing (e.g. mobility experience, always online, smarter/more personal experience).  
* The environment is changing (e.g. power, natural user input, and security/privacy).  
* Internet Explorer is 20 years old (IE6 was released 15 years, IE8 was released 7 years ago). 
![](https://cloud.githubusercontent.com/assets/5023024/9292258/a0c2802a-43b3-11e5-88b6-2bd1dc8639dd.JPG)  
* Legacy of Internet Explorer (IE 6: Strict vs. Quirks, IE 11: Engines render in all modes).  
* Edge doesn't include ```navigator.userAgent();```.  
![](https://cloud.githubusercontent.com/assets/5023024/9292263/cacab1c6-43b3-11e5-8b83-120302f1e5e3.JPG)  
* Instead, use [Modernizr](http://modernizr.com/) and pick features to turn on/off, instead of making browser exceptions. Modernizr is a JavaScript library that detects HTML5 and CSS3 features in the user’s browser.  
![](https://cloud.githubusercontent.com/assets/5023024/9292261/afe0e9c0-43b3-11e5-9123-15e7b3691ced.JPG)  

**Edge Advantages**:  
* Built for Windows 10. Managed through Group Policy → Mobile Device Management.  
* Ready to future with backwards compatibility.  

**Resources**:  
* [Microsoft Edge Platform Status](http:/dev.modern.ie/platform/status)  
* [Microsoft Edge Suggestions](http://tinyurl.com/EdgeUV)  
* [Microsoft Edge Developer Resources](http://dev.modern.ie)  
* [Edge Summit](http://tinyurl.com/EdgeSummit)  
* [Modernizr](http://modernizr.com/)
* [Windows 10: The First 24 Hours](http://blogs.windows.com/bloggingwindows/2015/07/30/windows-10-the-first-24-hours), article

### Adventures in Test-Driven Development ([Jeremy Lund](http://www.twitter.com/jeremy_lund))

**Why test?**:
* **“It's your job”** to make clean, well-tested code.
* **Testing clarifies your API and/or design.** The test becomes the first consumer of your code. It gives you ownership of the API/system you are building.
* **Your code becomes more resilient to change and refactoring** including performance and clarity.
* **Testing fixes the problems, not just the symptoms.**
* **TDD**: Test-driven development.
* **Red**: Write failing test → **Green**: Make a test pass → **Refactor**: Make it better!


Before going live with your application, and during the testing process **create a punch list**. For example:  
☑ ~~A container should be created~~  
☑ ~~The container should be closed by default~~  
❏  Clicking title...  
❏  ...  

**Writing a test**:  
**Arrange** (Given) → **Act** (When) → **Assert** (Then)  

**Quick Start**:  
Karma runs against browsers, and will be a *pending test* until a function is added. [Jasmine](http://jasmine.github.io) is added by default but [Mocha](https://mochajs.org) and [Chai](http://chaijs.com/) work, too.

```javascript
npm install karma -cli -g
npm init

npm install karma -D
karma init
```


### Keynote: The Current State of JavaScript ([Jon DeJong](http://www.twitter.com/jondejong))
**Things we can do Better:**  
1. **Testing:** Jasmine, Sinon, Mocha/Chai  
2. **Modules (Modular)**: Small modules that do *one* thing.  
3. **Testing**  
4. **Reusability** (yes, frameworks!)  
5. **Testing**  
6. **Clear dependency management**  
7. **Testing**  

*Build systems:*  
* Grunt
* Gulp
* Webpack

