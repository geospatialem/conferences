# Advanced IT Accessibility for Applications and Web Interfaces: State of Minnesota, January 2017 (St. Paul, Minn.)  

<img src="https://www.mn.gov/portal/assets/justified-logo_tcm1077-265308.jpg" width="25" alt="State of Minnesota logo"> [State of Minnesota](http://mn.gov)  

## Course Instructor:  
[Sarah Bourne](https://twitter.com/sarahebourne), [[Slides](<slidesLink>)] *slide link coming soon*  

## The old accessibility way  
We used to ignore it, leave it as-is, or say *I'll get to it later*...  

Which equated to:  
* **Winners**: nobody :frowning:  
* **Losers**: everybody :frowning:  



The old way of "doing accessibility"
Make (or buy) something.  Just before launch, throw it over the wall to the Accessibility Person.  Hand out tissues when it doesn't pass.  Make excuses about why it can't be fixed before launch when it turns out the Accessibility Person has no magic wand or pixie dust to sprinkle.
Winners: nobody
Losers: everybody
How to do accessibility better
The only way to fix this is to stop thinking that the Accessibility Person is the only one responsible for accessibility.  There is no way for any Accessibility Person to be an expert in all the technologies

Design Review: Vision Australia case study found 29 accessibility issues from JPEG template files – no coding!  But recommendations weren't implemented.  34 of 48 defects, or 70% of them, would have been avoided
The further back you can push accessibility thinking and decision making, the cheaper and better it is.  2005 data:
Average cost to find a bug on developer's desktop: $25
Average cost to find a bug during testing: $500
Average cost to find a bug by the customer: $15,000
Bonus: improves usability for everybody
Peer reviews catch 60 percent of the defects

Know HTML
Instead of spending time going over what accessibility is and why we care… let's go over the foundation of everything that's on the web.
Unlike programming languages, Hypertext Markup Language is designed to be forgiving.  If there are errors, browsers (aka "user agents") will make their best guess so they can display something.  This is why "it works on my computer" is not a good test at all.  Browser guessing is a rich source of intermittent errors, which why testing tools are so important.
HTML supports structural semantics (as opposed to content semantics- what the words mean).  It has elements for:
Organization and hierarchy of content: headings, lists, data tables, ARIA landmarks, HTML 5 sectioning elements
Identification of interactive features: hypertext links, form fields and controls
Identification of non-text content: images, image maps
HTML is designed to be accessible by default.  Use elements as they are intended and most of your work is done.  For content publishing, validating HTML can catch up to 95% of accessibility defects.  (For applications, your results may vary.)
If you use scripting magic in place of standard HTML elements, you have to make sure that it not only looks like the element, but that it behaves the same, and identifies itself the same to the browser so it can pass it to the operating system accessibility APIs.

Accessibility responsibilities by project role
Not everybody needs to know everything!  The more you know the better, but focus on the things you will be working on directly.
The more knowledge each contributor has about accessibility in their area:
the fewer defects they introduce,
the more opportunities for truly creative solutions that benefit everybody (Necessity is the mother of invention, or, constraints makes you think about things.)
the more satisfying it is to make things compliant, compared to bolting on stuff after the fact.

An exercise I worked on with MassIT folks: Mapping WCAG2 to Project Roles  Responsibilities can vary from project to project.  On smaller projects, some roles will be combined.  There may be roles not listed here.  The roles as used are defined at the end so you can adjust as needed.

Example: Who's responsible for alternative text?
Example for text alternatives for non-text content (e.g. images)
Content strategist:  guidelines for use of imagery and text
Graphic designer: identify images that are decorative
Content author:  write alternative text for informational images
HTML/CSS developer (prototype/development):  Determine whether to use CSS or null alt for decorative elements; use provided text alternative for informational images
Back-end developers: ensure place to store alternative text linked to images
No direct responsibility: business analyst, system architect, interaction designer.
Example by role – architect.
24 success criteria (40 with AAA)
Multimedia use: identify video players/platforms that can support captions, audio description, operable controls
Ensure script libraries and plugins support keyboard-only use, controls for motion,  language of parts, correct use of HTML including form elements, and error handling
Pain avoided: picking a script library for widgets that can't be made accessible and having to start over
Example by role – graphic designer.
25 success criteria (42 with AAA)
Design visual elements that reflect semantic structure and reading and interaction flows
Design effects for indicating focus and selection and for displaying error messages
Design controls for operating multimedia, audio, motion, skip to content, etc.
Identify decorative non-text elements
Avoid use of visual only design cues
Ensure color is not sole indication of meaning
Ensure color palette supports good contrast
Specify fonts (not pictures of text)
Pain avoided:  Problem with contrast after executive stakeholders have already approved font, etc., colors
Example by role – content author.
23 success criteria (35 with AAA)
Use hierarchical heading to organize content
Provide text alternatives for non-text elements
Write link text, form labels, error messages, page titles, section headings, and other "microtext"
Write/edit captions and transcripts for multimedia
Don't misuse HTML for layout or other visual effects
Avoid use of visual references, such as color or location on screen.
Pain avoided: Embarrassing error messages and alternative text, delays in publishing to fix errors and introduced defects
Example by role – developers.
38 success criteria (59 with AAA) (aka, everything)
Not always "responsible", but:
Need to know how to implement
Will be the first one to catch errors (unit testing)
Will be the one who has to do all the re-work
All the things boil down to:
Know HTML and use correct and valid markup
Understand how operating system accessibility APIs interact with browsers, and how that works in the context of the DOM
Pain avoided:  Re-work
Other roles, other responsibilities
Not all project roles are on the chart
Executive stakeholders
Understand requirement for accessibility
Top-down communication of support for accessibility
Governance and culture
Program and project managers, from planning and procurement through development and deployment.  They are not responsible for specific WCAG guidelines, so don't need to know the technical aspects of how to comply.  But they do need to know who should know, where to expect what kind of testing, and facilitating governance and controls matters. Culture: empower team members to work with responsible parties.
Accessibility Person: Shared resource across all projects.  Provide technical guidance when needed, and advise on where to get more expertise, ad hoc and formal training, sustaining management support, contribute to process improvements, manage policies and standards

Agile   
Ways agile can undermine accessibility:
Decentralized ownership weakens top-down mandates
Teams control their own "backlogs" (aka, to-do list)
Means shiny new features more likely to win out over accessibility fixes
Agile methodologies can actually improve accessibility:
More incentives for integration of accessibility responsibilities
Better mechanisms for ensuring testing happens early and often
How to:
Include accessibility at Inception phase
Include accessibility in your definition of "ready" and "done"
Create accessibility-related tasks (primarily testing)
Test Driven Development: define testing req for each sprint
Design/UX sprints ahead of or parallel to development sprints
Include accessibility acceptance criteria in Backlog Stories
Requirements: wireframes and comps need to be marked-up, annotated
Make sure each scrum team has accessibility knowledge (if not expertise)
Focus on creating accessible reusable components
Build accessibility into testing framework
Give every developer testing tools they can run themselves at any time in their own browser (Everybody would rather find their own mistakes themselves)
Use automated testing for everything you can and opt everyone in
Perform manual spot checks
Track everything

Testing approaches and tools by project phase
Testing by project phase - Solution selection
Selecting products and 3rd party add-ons: to determine baseline accessibility so you know which features to avoid or that will have to be fixed in development
Make accessibility a requirement
Request accessibility information: test reports, developer guidance
Search for references to accessibility on the web, customer forums
Run accessibility tests on a demo or free trial site
Identify problems
Identify possible solutions: features to avoid, customizations needed, etc.
Include mitigation and remediation costs in decision-making
Useful testing tools:
keyboard test
WebAIM’s WAVE toolbar (Chrome add-on)
other developer tools

Testing by project phase - Design and development
Objectives of testing during design and development:
Find and fix as many defects as early as possible
Make sure an audit test does not turn up surprises
Learn from results: continuous reduction of defects
A Very Large project in MA went from dozens of defects on every page to less than two each, none of which were "blockers" (non-critical defects).  Cheapest bug fix is the one you don't have to make.
Selecting testing tools:
So many! And most are free. See the W3C Web Accessibility Evaluation Tools List
Be sure they test pages as rendered when using JavaScript, rather than source code
Pick tools that are compatible with your existing systems and workflows:
Project management
Testing framework
Bug tracking
Testing by project phase - Design
Because there is rarely rendered code to work with, testing by checklist provides most value
Identify WCAG2 guidelines that pertain to create checklist
Annotate comps and wireframes with accessibility requirements
Identify headings and correct nesting, lists, data tables and their headers
Document content flow order
Identify non-informational images
Etc.
Useful testing tools:
Color contrast tests (Color Contrast Analyzer, Colour Contrast Analyser (CCA), Juicy Studio Accessibility Toolbar, Vischeck, etc.)
Palette builders and tests (Accessible color palette builder, A11y Rocks Color Palette, etc.
Colorblindness simulators (Vischeck, Color Oracle, etc.)

Testing by project phase – Development
Keyboard testing
Ensures usability for keyboard-only users, people who use specialized input/output hardware , and as a first check for software assistive technology compatibility.
Look for:
correct content flow
all links and form elements can be reached and used
visual indication of where you are
no "keyboard traps"
expected behavior of modal/dialog boxes and other pop-ups.
Quick, easy to learn, and no license fees.
Every developer should know to do keyboard testing before checking in code!

Testing by project phase – Development, 2
Automated testing
Automated test can only definitively test for 25-30% of WCAG criteria, but catches 50% or more of defects.
But tend to be the most frequently found defects in audit testing.
Testing tools can help with things that can’t be fully automated
Correct alternative text – finds all the images, then you judge.
Correct nesting of headings –  finds all the headings, then you judge
Manual tests
Manual techniques for other requirements
code inspection
keyboard operation
testing with screen readers, magnifiers, and voice recognition.
Use automation to track when you really need to do manually testing again
 – only when a change for something that was caught by manual testing.
Testing by project phase – Development, 3
Assistive Technology testing
Ensure everything works as intended; check on verbosity
Does not provide diagnostics: you may learn that something doesn't work, but you don't learn anything about why.
AT testing matrix: TEST ALL THE THINGS … is not realistic.
At some point, all you're doing is testing for bugs in any/all of those rather than accessibility issues.
Trim by looking for redundancies can often get to 10 AT/OS/browser combinations
Look for redundancies (for instance, if VoiceOver works on an iPhone, it's going to work on a Mac desktop) to reduce.
Add special cases when you know what people are actually using
(such as employees.)
4 operating systems, 2 supported versions each
5 assistive technologies
4 browsers, 2 supported versions each
3 responsive breakpoints
216 combinations – before adding devices!

Testing with AT users (designers and developers)
Ensures compliance with standards actually results in something usable
Helps determine impact of known technical defects
Don't waste their time with testing that a machine can do faster and better.
Testing by project phase – Development, 4
Desktop Testing with Firefox:
Needs updating because some tools aren't available on Firefox anymore, but approach is still valid.  
Designed to be in an efficient order for testing rather than by WCAG numbering.
Can be used for solution evaluations, unit testing, integration testing.
Test as you go: browser add-ons and bookmarklets
The best ones are the ones that work the best for you for what you’re doing
WebAIM’s WAVE toolbar: checks and educates at the same time
Web Developer Toolbar: dozens of checks, many of which useful for accessibility
Firebug or browsers’ “Inspect element” feature
W3C Web Accessibility Evaluation Tools List
Bookmarks on CommonWiki for:
Testing tools and color testing tools
Testing techniques
Testing by project phase – User Acceptance
Audit testing
Akin to IV&V, using third-party or other trusted testers.  MA has a master contract for this.
Audit testing usually not done until user acceptance, so big incentive to do good testing during development.
Do earlier if working with very complex systems or cutting-edge technologies, and plan on re-testing
Agile:
Have audit test done before first public release.
Additional audit tests
As indicated from analysis of bug records from your testing
When major new features are added
For new reusable components are added
When significant changes to major features and reusable components
Assessing and prioritizing accessibility problems
All software has bugs.  Not all defects are equal.  The goal is to prioritize the ones that create an unequal experience for people with disabilities.
Who are your users?
You have more options to provide accommodations and training for employees than for the general public.
Use a severity ranking
A good way of determining the overall severity of various defects is to look at both occurrence, or frequency, and impact on users.
Occurrence or frequency of a defect:
Determine the occurrence or frequency of a defect by looking at how many times a user is apt to come across it. For instance:
Low: Defect only found in one or a few places
Moderate: Defect appears in multiple places
High: Defect appears in many places
Significant: Defect appears throughout
Impact a defect has:
Determine the impact a defect has on a user's ability to use a particular feature or function. For instance:
Low: The defect has little or no impact on end-users
Moderate: Annoying, but has a minor end-user workaround
High: An annoying defect that has an onerous or confusing end-user workaround
Significant: The defect prevent an end-user from performing the function

Combining the scores for occurrence and impact should allow you to prioritize the defects. Since there is some subjectivity involved, actual users of AT should be asked to review the results as a reality check.
Assessing and prioritizing accessibility problems, 2
The next step is to identify potential remedies for the prioritized accessibility problems. These could include:
Identify remediation or mitigation options, such as
fixing the code
reconfiguration
identifying and documenting workarounds
shutting off unneeded features
providing an alternative and equitable means of online access
Gather data for options on:
Gather data for the identified options that will aid in decision-making, such as how long it will take to implement, the level of effort and types of resources it will take, and implied short- and long-term commitments. You also need to identify mitigation efforts that will be required until remediation is completed, along with associated costs.  (Tip: workarounds and alternatives usually end up costing more than just fixing them, but may need to be considered for commercial products.)
how long it will take to implement
level of effort and resources it will take
implied short- and long-term commitments and their costs
cost of interim mitigation efforts
Assessing and prioritizing accessibility problems, 3
Consider cost, timing, operational impacts, and feasibility in terms of the project overall.
Consider contractual obligations
At this point you will have concrete data that can be used in making decisions, such as assigning resources to IT systems and services, prioritizing in an agile backlog, or as part of a procurement process.
The last phase is to consider cost, timing, operational impacts, and feasibility. At this point, you will analyze the data gathered while ranking severity and investigating remediation and mitigation options to determine the most beneficial approach to addressing identified accessibility problems.  At this point you will have concrete data that can be used in making decisions, such as assigning resources to IT systems and services, prioritizing in an agile backlog, or as part of a procurement process.
Procurement and contracting strategies so you don’t buy problems
Last but not least, don't buy problems, or if you do, make sure your contracts include required accessibility activities to minimize the impact on users with disabilities, with ways to measure that they are done effectively.
Requires a commitment to project and contract management.  It seems that many people think only lawyers and procurement staff need to look at contracts.
Goal: don’t buy problems without planned or contracted solutions
Follow your procurement rules for accessibility
Requires a commitment to project and contract management.
Evaluate solutions and bids before deciding
(See also: previous slide, “Testing by project phase - Solution selection”)
Evaluating solutions/bids
You may need to make decisions before you have results of third party testing or other hard data. The following are resources that may be available where you can get information on accessibility of products or services.

The Voluntary Product Accessibility Template®, or VPAT®, is a tool used to document a product's conformance with the accessibility standards under Section 508 of the Rehabilitation Act.
Because VPATs are produced by the vendors:
tod idea to rely on comparing VPATs from different vendors
The information in a VPAT should be considered a starting point
VPATs only report on a specific product
Note: Just having a VPAT does not mean the product meets accessibility requirements.
Evaluation - Online and other vendor support
Online and other vendor support:
Many vendor provide forums, wikis, and other online resources for customers. These are great places to see if customers are having accessibility-related problems and what solutions or workarounds are available.
Vendors may also have technical guidance published, including integration and customization directions to ensure developers do not introduce new accessibility issues or inadvertently disable existing accessibility features.
List of open accessibility tickets and their status
If not published, be sure to ask vendors if they have any accessibility fixes or enhancements scheduled for future releases.
Evaluation - Accessibility maturity
Accessibility maturity
Ask vendors questions that can help you gauge how much expertise a vendor has and the level of commitment they make to building accessibility into their products. This may help you evaluate documentation they have provided and remediation options. Examples include:
Do you include accessibility requirements in your design and development processes?
Do you have accessibility experts in your design and development teams?
What kind of accessibility training do you provide for your designers and developers?
Do you have an in-house accessibility testing facility?
Do you use an external company with accessibility expertise?
Who does the testing for your test results documentation, such as your VPAT?
Do you participate in any accessibility-related standards-setting groups?
What is the handling and escalation process for accessibility-related problems found by customers?
Evaluation - Accessibility maturity, advanced
Or, see  Policy Driven Adoption for Accessibility (PDAA)!
A formalized approach to asking those questions and evaluating the responses
Hatched as a multi-state effort.
Pilots in Minnesota and Texas
Ask Jay Wyant to learn more.
