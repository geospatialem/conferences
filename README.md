# Notes from Conferences
Below is a list of notes compiled by [Kitty Hurley](http://www.twitter.com/geospatialem) from various conferences.

* MidwestJS 2015


## [MidwestJS](http://www.midwestjs.com) 2015, Minneapolis, Minn.

Midwest JS is a premier technology conference focused on the JavaScript ecosystem. There were a variety of talks from well­known speakers in the community in a typical presentation format. Talks were categorized and structured based on the following tracks:

* Beginner Track (JavaScript fundamentals, jQuery, jQuery UI, etc.)
* Frameworks Track (Angular.js, Knockout.js, Ember.js, Backbone.js, etc.)
* Node Track (anything based on Node.js)
* Mobile­Track (PhoneGap, Appcelerator, etc.)
* Testing Track (TDD, Jasmine, etc.)
* Miscellaneous Track (Anything that doesn't fit into the others)

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

Resources:
* [Structure and Interpretation of Computer Programs](http://www.amazon.com/Structure-Interpretation-Computer-Programs-Engineering/dp/0262510871), book

#### Writing Better jQuery-Infused JavaScript ([Ken Dale](http://www.twitter.com/kendaleiv))
Text

#### Components are the Future of the Web: It's Going to be Okay ([Tessa Thornton](http://www.twitter.com/tessthornton))
Text

#### Debugging in Chrome (Josh Longanecker)
Text

#### Development for FirefoxOS: Web ([Dan Callahan](http://www.twitter.com/callahad))
Text

#### That's so Prototypical ([Jordan Kasper](http://www.twitter.com/jakerella))
Text

### Friday, August 14th, 2015
#### Enterprise JavaScript Apps with Typescript ([Kurt Wiersma](http://www.twitter.com/kwiersma))
Text

#### JavaScript Forensics ([Todd Gardner](http://www.twitter.com/toddhgardner))
Text

#### Test Them Puzzles ([Branden Byers](http://www.twitter.com/brandenbyers))
Text

#### Edge of Tomorrow ([David Giard](http://www.twitter.com/davidgiard))
Text

#### Adventures in Test-Driven Development ([Jeremy Lund](http://www.twitter.com/jeremy_lund))
Text

#### Keynote: The Current State of JavaScript ([Jon DeJong](http://www.twitter.com/jondejong))
Better:  
1. Testing: Jasmine, Sinon, Mocha/Chai  
2. Modules (Modular): Small modules that do *one* thing.  
3. Testing  
4. Reusability (yes, frameworks!)  
5. Testing  
6. Clear dependency management  
7. Testing  

Build systems:
* Grunt
* Gulp
* Webpack
