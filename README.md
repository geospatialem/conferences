# Notes from Conferences
Below is a list of notes compiled by [Kitty Hurley](http://www.twitter.com/geospatialem) from various conferences.

## 2015
* [MidwestJS](#midwestjs-minneapolis-minn)


## [MidwestJS](http://www.midwestjs.com), Minneapolis, Minn.

Midwest JS is a premier technology conference focused on the JavaScript ecosystem. There were a variety of talks from well­known speakers in the community in a typical presentation format. 

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
* *[Enterprise JavaScript Apps with TypeScript](#enterprise-javascript-apps-with-typescript-kurt-wiersma)**, Kurt Wiersma  
* *[JavaScript Forensics](#javascript-forensics-todd-gardner)*, Todd Gardner  
* *[Test Them Puzzles: What Test-Driven Learning Can Teach About JS and TDD](#test-them-puzzles-what-test-driven-learning-can-teach-about-js-and-tdd-branden-byers)*, Branden Byers  
* *[Edge of Tomorrow: Introducing Microsoft's New Browser](#edge-of-tomorrow-introducing-microsofts-new-browser-david-giard)*, David Giard  
* *[Adventures in Test-Driven Development](#adventures-in-test-driven-development-jeremy-lund)*, Jeremy Lund  
* *[Closing Keynote: The Current State of JavaScript](#keynote-the-current-state-of-javascript-jon-dejong)*, Jon DeJong  


### Thursday, August 13th, 2015
#### Keynote: The Art of Simplicity ([Venkat Subramaniam](http://www.twitter.com/venkat_s))
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
1. **Simple's not clever**: It is a realization, a *clear solution!!* How do we manage code when there is no logic? Would you do this to your children, name them ```p```? We lose abstraction of our ideas.  
2. **Simple's not necessarily familiar**: *(aka accidential complexitivity)* Something may be complex for a minute. Familiarity can look, or even be complex, it's all about understanding. One hard realization is the *self-inflicting wound pattern*, when we forget to do something one day, and it continues to build up over time. Focus on: *what* you are doing, don't confuse, and use *declarative* code (it's simpler)! See: [Venkat's blog post](http://blog.agiledeveloper.com/2015/08/prefer-functional-style-over-imperative.html) for an example of functional vs. imperative code. Simple has fewer moving parts, illuminate them!       
3. **Simple's not over-engineered**: See: *the automated back scratcher comic strip*. (e.g. a phone call with someone in the room vs. an in-person discussion).    
4. **Simple's not terse**: Don't confuse simple/concise with terse. It's about extensibility. Terse vs. concise: *Terse* is short, and waiting to hurt you when you least expect it. (e.g. See *code victim screenshot*). *Concise* is transparent. If you don't know why your application in production is failing every three weeks, find out why and break down the steps.  
5. **Simple keeps you focused**: Focus keeps down the distractions. (e.g. Search Engines: Yahoo has news distractions, *why did we come here again?*, Bing is beautiful, *do we really want to search and lose this beautiful picture?*, and Google is simplistic, we don't get lost in anything, *let's start our search*). This is extremely hard to do, to do something simple. It is *extremely valuable* to value someone else's time. Focus on the user, and don't distract them. This takes *genius* and *courage*.  
6. **Simple fails less**: (e.g. Manhole's shape is a circle, one size fits all)!  
7. **Simple's easy to understand**: Simple is easy to work with!  
8. **Simple is elegant**: Fluancy., or code that doesn't look like a tornado! When there is nothing to take the focus away from something, it is truly elegant (e.g. Mona Lisa painting). This presents the *Architect's dilemna* (e.g. Trinity Church and an adjacent building in Boston, Mass' reflection off the church).  
9. **Simplicity has to evolve**: We have all said, *my code simply sucks* at some point. Over time, things change, and as we change, simplicity will as well. Simple makes things easy, but its certainly not easy.  

**Resources:**  
* [Structure and Interpretation of Computer Programs](http://www.amazon.com/Structure-Interpretation-Computer-Programs-Engineering/dp/0262510871), book

#### Writing Better jQuery Infused JavaScript ([Ken Dale](http://www.twitter.com/kendaleiv)),  [Slides](http://kendaleiv.com/jquery-js-refactor/#/)  

**Keys for Maintainability/Testability/Warm Fuzzies:**  
1. **External files** (Good practice): Caching JavaScript in-browser.  
2. **Strict mode** helps troubleshooting.  
3. **Wrap in Life**: Function wrapped in params ```(``` and ```)```. This *thing* will immediately execute. This will shield the library from tampering (which is useful with global variables). Good resource [Atom editor](https://atom.io) (Windows/Apple).  
4. **Shorthand Luke**: Using document.ready, changing ```click``` → ```on```, changing ```success``` → ```done``` (JavaScript process/chaining). Avoid deprecated items (see jQuery [docs](https://api.jquery.com/category/deprecated)).  

**Other Notes:**
* If you're having a problem up front, thats normal.
* **Refactoring**: AJAX provides data and is a ```promise``` in itself.  
* **Testing**: e.g. Jasmine for Frameworks/Libraries. Test descriptions with ```it``` using ```expect``` and ```toBe``` statements. There are custom Jasmine matches, such as ```spyOn``` (see [documentation](http://jasmine.github.io)).  
* **DRY** test your code (aka **D**on't **R**epeat **Y**ourself). The opposite of DRY testing is **WET** (aka **W**e **E**njoy **T**yping). Ideally have one single representation in your code base.
* **Other ways:** requireJS, ES6 modules (which may be the future), etc.
* **Start**: 44 lines of code. **End:** HTML: 25 lines, JS: 127 lines. *Sometimes simplicity requires more lines of code*, for troubleshooting and for helping ourselves in the future. Used the Jasmine HTML runner.

**Resources:** 
* [Code](http://www.github.com/kendaleiv/jquery-js-refactor): Check out the commits to see the refactoring process from start → finish.
* [Slides](http://www.kendaleiv/jquery-js-refactor/#/)

#### Components are the Future of the Web: It's Going to be Okay ([Tessa Thornton](http://www.twitter.com/tessthornton))  

* HTML is semantic (clean and virtuous)
* We haven't kept up on complex UI's
* HTML is not just for content (e.g. adding in JSON files from JavaScript into HTML). HTML isn't just for content, and it never was.
* **Imperative**: the steps to achieve a desired result *versus* **Declarative**: the desired result, leaves the implementation up to something else (e.g. SQL).
* HTML has declarative API's, or a contract of inputs + outputs. HTML needs to know what to put in it, which is especially true in HTML5.
* We're writing JavaScript like we don't have any control over HTML. 
* In 2009, AngularJS was created with the idea of seperating HTML from the DOM, the *seperation of concerns*. Not just one implementation. We can make our own delcarative **attributes** and **elements**.
* The future will focus content with HTML and action with JavaScript, specific actions wired together to focus on your application.
* You're going to *pollute* your HTML and you're going to like it!

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

#### Better Debugging in Chrome (Josh Longanecker)

**Tricks + Tips**:  
* **Scroll into view** from code → browser.  
* **Awaits** tab: Will showcase the performance on your code.  
* **Pretty Print**: under ```Sources``` → ```{}``` in the lower-left.  
* Press ```Ctrl``` + ```Shift``` + ```f```: to see all functions.
* **Breakpoints**: Conditional breakpoints, lists breakpoints to turn on/off in the right-hand window, step over breakpoints.
* **Blackbox script**: The debugger will ignore scripts. To enable right-click the JavaScript file.
* **Console.log(); messages**: ```console.error();```, ```console.log();```, ```console.group();```, ```console.groupEnd();```, ```console.groupLog();```, ```console.groupCollapsed();```, ```console.assert();```, etc.
* **Preserve log**: Good practice when testing out AJAX calls (Before/After)
* **Timeline**: ```console.time();``` and ```console.timeEnd();```.

**Resources:**  
* [Chrome documentation](https://developer.chrome.com/devtools)  

#### Developing for Firefox OS: It's just the Web... or is it? ([Dan Callahan](http://www.twitter.com/callahad))  
Mozilla is working with smartphones and tv's solely using web development.

**Resources:**  
* [Mozilla Developer Network](https://developer.mozilla.org/en-US)
* [Firefox Developers](http://www.firefox.com/developer): Add instance developer *(currently in Beta)*

#### That's so Prototypical ([Jordan Kasper](http://www.twitter.com/jakerella))
Text

### Friday, August 14th, 2015
#### Enterprise JavaScript Apps with TypeScript ([Kurt Wiersma](http://www.twitter.com/kwiersma))
Text

#### JavaScript Forensics ([Todd Gardner](http://www.twitter.com/toddhgardner))
Text

#### Test Them Puzzles: What Test-Driven Learning Can Teach About JS and TDD ([Branden Byers](http://www.twitter.com/brandenbyers))
Text

#### Edge of Tomorrow: Introducing Microsoft's New Browser ([David Giard](http://www.twitter.com/davidgiard))
Text

#### Adventures in Test-Driven Development ([Jeremy Lund](http://www.twitter.com/jeremy_lund))
Text

#### Keynote: The Current State of JavaScript ([Jon DeJong](http://www.twitter.com/jondejong))
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
