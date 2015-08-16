# MidwestJS 2015 (Minneapolis, Minn.)

[Midwest JS](http://www.midwestjs.com) is a premier technology conference focused on the JavaScript ecosystem. There were a variety of talks from well­known speakers in the community in a typical presentation format. 

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
* *[Enterprise JavaScript Apps with TypeScript](#enterprise-javascript-apps-with-typescript-kurt-wiersma)*, Kurt Wiersma  
* *[JavaScript Forensics](#javascript-forensics-todd-gardner)*, Todd Gardner  
* *[Test Them Puzzles: What Test-Driven Learning Can Teach About JS and TDD](#test-them-puzzles-what-test-driven-learning-can-teach-about-js-and-tdd-branden-byers-slides)*, Branden Byers  
* *[Edge of Tomorrow: Introducing Microsoft's New Browser](#edge-of-tomorrow-introducing-microsofts-new-browser-david-giard)*, David Giard  
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

### Writing Better jQuery Infused JavaScript ([Ken Dale](http://www.twitter.com/kendaleiv)),  [Slides](http://kendaleiv.com/jquery-js-refactor/#/)  

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

### Components are the Future of the Web: It's Going to be Okay ([Tessa Thornton](http://www.twitter.com/tessthornton))  

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

### Better Debugging in Chrome (Josh Longanecker)

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
### Enterprise JavaScript Apps with TypeScript ([Kurt Wiersma](http://www.twitter.com/kwiersma))

* **JavaScript is a valid typescript**
* It takes discipline to write good code.
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
tsc --sourcemap --our js/Application.js js/_all.ts
```

**Making a Better Application**:
* Gradually move JavaScript to TypeScript.
* Add types, a better way to structure code along the way.
* Can make working with an API easier to learn.

**Resources**:
* [Angular in 20 minutes](https://github.com/DanWahlin/AngularIn20TypeScript)
* Expense Manager (*link coming soon*)

### JavaScript Forensics ([Todd Gardner](http://www.twitter.com/toddhgardner))
Text

### Test Them Puzzles: What Test-Driven Learning Can Teach About JS and TDD ([Branden Byers](http://www.twitter.com/brandenbyers)), [Slides](http://brandenbyers.com/slides/test-them-puzzles)

* **Learning to code is hard,** puzzles are a great way to make it fun.  
* We need that **Aha! Dopamine drip moment**, they are important! The more we do it and achieve these moments the more exciting and rewarding it gets!  
* An hour is a good time for digesting a puzzle. If you can't solve it, put it off to the side and try again. When you do solve it, you'll get that Aha! moment, see any hurdles from the past, and/or question why it was a harder problem before.  
*  Puzzles are nimble.
*  It's hard to describe in a simple way (see: Puzzle test below).
*  I don't know how to solve it, but I can think about the problem and how to approach it.  
*  Think of things in **bite-size chunks**.  
*  Syntactic Wilderness: Wander and you might get lost.   
*  Think of the test as the end-product itself.  
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
* Inquisitive  
* Destructive exploration  
* Playful learners  
* Pull, tear, scratch, probe  
* Haphazardly dig for food  

**Crows**:  
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
* [Rosetta Code: Towers of Hanoi](http://rosettacode.org/wiki/towers_of_hanoi) 
* [Flexibility in Problem Solving and Tool Use of Kea and New Caledonian Crows in a Multi Access Box Paradigm](http://journals.plos.org/plosone/article?id=10.1371/journal.pone.0020231), article (Parrots and crows)  

### Edge of Tomorrow: Introducing Microsoft's New Browser ([David Giard](http://www.twitter.com/davidgiard))
Text

### Adventures in Test-Driven Development ([Jeremy Lund](http://www.twitter.com/jeremy_lund))
Text

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
