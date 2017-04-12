# Debugging JavaScript, April 2017 (Minneapolis, Minn.)  

<img src="https://cloud.githubusercontent.com/assets/5023024/24884789/b5862bb8-1e10-11e7-9c1c-53b5cadb89ef.png" width="45" alt="Front End Masters logo"> [Front End Masters](http://mn.gov)  

## Course Instructor:  
[Todd H Gardner](https://twitter.com/toddhgardner)  

## Miscellaneous Notes  
* JavaScript happens
* Emoji is 2 bytes (unicode characters)  
* _"Debugging is like being the **detective** in a crime movie where you're also the **murderer**."_ -Filipe Fortes
* Bugs are from [GetRantr](https://github.com/toddhgardner/getrantr), built on Backbone.js, and reside in the following files:
```
src → public → index.html
src → public → signup.html
src → public → scripts
```

## How to Fix Bugs  
**1) Identify → 2) Isolate → 3) Resolve → 4) Prevent**  

### 1) Identify  
The earlier you catch a bug, the:
* Cheaper  
* Better  
* Faster  

|                | Stage          | Stage Name     |
| :------------- | :------------- | :------------- |
| ↑              | Earliest       | Development    |
| ↑              |                | Testing        |
| ↑              |                | Monitoring     |
| ↑              | Latest         | User Reports   |

### 2) Isolate  
#### Context
* Browser
* Page
* User
* Script(s)    

#### Timeline of events
* Complex state machine  
* API(s)  
* JavaScript applications  
* DOM  
* Browser  

#### Root cause of why  
* Symptoms
* State  

### 3) Resolve  
Risk, Change, Impact, and "The Right Way"

_"How risky is it to deploy to you?"_

### 4) Prevent  

#### A. Regression tests  
Tests to check for the recurrence of a bug

#### B. Process change  
* Manual  
* Automated  

#### C. Do nothing  
Tests and process have cost. Don't increase them trivially.  

## Bug 1: Delete rant  

### Problem
A user is unable to delete a rant.  

### Troubleshooting  
Use the **Preserve log** checkbox and using the DOM inspector click the Delete button, and navigate to the `Event listeners` and `Ancestors` checkbox.  

The button in form submit (JavaScript by default) is preventing the default action.  

Using Async, determine the files linked to the system files with the console. Blackbox scripts to limit them from the list (good for libraries). Blackboxing adds a banner to the top of the file so you know it is blackboxed.  

Step through using breakpoints and scope.  

### Solution
It's a logical bug where the event is a `PreventDefault`. The function content (value of `this`) in the `scripts/rantListView.js` file.

Use `bind` to force the value, guaranteeing it is saved. _Note: This can only be used once._

```javascript
/* Bug 1: Before */
//   onDelete: function() {
//     setTimeout(function() {
//       console.log(this.model);
//       this.model.destroy();
//       this.remove();
//     });
//   }

/* Bug 1: After */
onDelete: function() {
  setTimeout(function() {
    this.model.destroy();
    this.remove();
  }.bind(this)); // Bind forces this to be saved (Note: Can only be used once)
}
```

### Concepts  
* Keystone users  
* DOM inspector  
* Async callbacks  
* Blackbox scripts  


## Bug 2: Rant text remembered after deleted   

### Problem
<text>

### Troubleshooting  
<text>

### Solution
<text>


```javascript  
/* Before: Bug 2 */
// if (text) {
//   localStorage.setItem('next-rant', text);
// }

/* After: Bug 2 */
//console.log(text); //Testing the text
if (typeof text === 'string') { //Check if the text is a string, if it is, then save the rant text (if deleted it won't be a string)
  localStorage.setItem('next-rant', text);
}
```

### Concepts  


## Bug 3: Monitoring, Server reporting, and lots of 400 requests (200+)  

### Problem
<text>

### Troubleshooting  
<text>

### Solution
<text>

**HTML**:  
```html  
<!--Before Bug 3-->
<!-- <textarea id="rant_text" name="rant" placeholder="Well, actually..."></textarea> -->

<!-- After: Bug 3-->
<textarea id="rant_text" name="rant" placeholder="Well, actually..." required=""></textarea>
```

**JavaScript**:  
```javascript  
/* Before: Bug 3*/
//     analytics.trackConversion();
//     this.collection.create(rant, { wait: true });

//     form.rant.value = '';

/* After: Bug 3*/
if (rant.text && rant.text.length > 0) { //Add user form validation if the text length is greater than 0 characters
  analytics.trackConversion();
  this.collection.create(rant, { wait: true });

  form.rant.value = '';
}
```

### Concepts  

## Bug 4: Single user 2,124 errors ('substr' of null)  

### Problem
<text>

### Troubleshooting  
<text>

### Solution
<text>

```javascript  
/* Before: Bug 4 */
//   render: function() {
//     this.$el.html(this.template(this.model.toJSON()));
//     return this;
//   },

  /* After: Bug 4 */
  render: function() {
    var rant = this.model.toJSON();
    if (typeof rant.text == "string") { //Add a validation message to the user, if something doesn't look right
      console.error("invalid rant data", rant);
      rant.text = "Sorry! An error occurred with this rant. Our team is on it!";
    }
  },
```  

### Concepts  

## Bug 5: Unexpected high memory usage  

### Problem
<text>

### Troubleshooting  
<text>

### Solution
<text>

```javascript  
/* Before: Bug 5 */
//   render: function() {
//     this.$el.html('');
//     this.collection.each(this.renderStatement, this);
//     return this;
//   },

 /* After: Bug 5 */
  render: function() {
    this.el.innerHTML = '';
    this.children.forEach((view) => { view.remove(); }); //Cleanup eachc child (Optional)
    this.children.length = 0; //Zero out the array, "release children for garbage cleanup"
    this.collection.each((model) => {
      this.renderAd(model);
    });
    return this;
},
```

### Concepts  

## Bug 6: Slow to load page    

### Problem
<text>

### Troubleshooting  
<text>

### Solution
<text>



### Concepts  

## Bug 7: Form.Submit not a function on signup (343 errors)    

### Problem
<text>

### Troubleshooting  
<text>

### Solution
<text>

```html  
<!-- Before: Bug 7 -->
<!-- <div class="signup-action text-center">
  <button type="submit" name="submit" class="btn btn-lg btn-orange">Start My Free Trial</button>
</div> -->

<!-- After: Bug 7 -->
<div class="signup-action text-center">
  <button type="submit" class="btn btn-lg btn-orange">Start My Free Trial</button>
</div>
```

### Concepts  

## Bug 8: Network is not defined  

### Problem
<text>

### Troubleshooting  
<text>

### Solution
<text>

**HTML**:  
```html  
<!-- <script type="text/javascript" src="http://cdn.getrantr.com:9000/vendor/analytics.js"></script> --> <!--Bug 8 commented out -->

<!-- <script type="text/javascript" src="http://cdn.getrantr.com:9000/vendor/jquery.js"></script> --> <!-- Bug 8 commented out -->
```  

**Check if jQuery loaded**:  
```javascript  
/* Bug 8: Check if jQuery has loaded */
if (!window.$) {
  console.error('Failed to load jQuery dependency.');
  document.body.innerHTML = '<h1 style="color: red;">Sorry! An error occurred loading the application. Please try again.</h1>'; //Let the user know
  //Could also add in an email address, if multiple issues occur.
}
/* /Bug 8 */
```

**Check if analytics.js loaded**:
```javascript  
/* Before: Bug 8 */
  // if (rant.text && rant.text.length > 0) { // <-- add this validation check
  //   analytics.trackConversion();
  //   this.collection.create(rant, { wait: true });
  //
  //   form.rant.value = '';
  // }

  /* After: Bug 8*/
    if (rant.text && rant.text.length > 0) { // <-- add this validation check
      //If analytics loaded in properly
      if (window.analytics) { //Since its a global
        analytics.trackConversion();
      }
      this.collection.create(rant, { wait: true });

      form.rant.value = '';
    }
  }
```

### Concepts  

## Design for Debuggability  
**1) Identify → 2) Isolate → 3) Resolve → 4) Prevent**  

### 1) Identify  
Identify early for cheaper, better, and faster results:

|                | Stage          | Stage Name     |
| :------------- | :------------- | :------------- |
| ↑              | Earliest       | Development    |
| ↑              |                | Testing        |
| ↑              |                | Monitoring     |
| ↑              | Latest         | User Reports   |

#### Monitoring tools  
Track.js and Elastic  

#### Instrument  
Priorities (for page load and time)   

### 2) Isolate  
Simplicity is key and should be the core idea of the application. Design for testing (hardware).  

#### Rule of Three   
1. Solve it once  
2. Solve it again  
3. Abstraction  

#### Debug Mode Tools  
* http://myapp.com?debug  
* Chrome  
* SauceLabs (Remote testing on browsers and OS)  
* Charles/Fiddler  
* Track.js  

### 3) Resolve  
Lower the risk of change (e.g. pacemaker software vs. low hit web application). Build quality software with **testing, testing, and more testing**. Have users test your application in and under development.  

### 4) Prevent  
**_Think!_** Use regression tests, update process, and/or do nothing. Use bug count as a proxy for **Design quality**.

#### Design quality  
Abstraction ↓ **Simplicity** ↑ Duplication

### Generic Architecture
Request → The doer thing → Widgetizer → Enterprise-ready Cylinder _or_

Request → The doer thing → Powerful cloud → Enterprise-ready Cylinder
