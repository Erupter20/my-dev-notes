**day 0, web basics**
1. networking
2. client server architecture
3. example of ordering a meal and comparing it to client-server architecture.
4. Each time you make a request, you get a response. Not getting a response is also a response
5.  client (front-end) is connected to backend via a bridge(API), driver to connect to database with backend (client-server architecture)
	establishing connecting, between client server, TCP(acknowledgement at every step, end-to-end encryption, hard to hack) vs UDP(no acknowledgement, no encryption, easy to hack)

5. What do we get in response? -> internet is connected in wires -> data travels to packets -> let's say those are html,css,js -> merged by "BROWSER" using PARSERS(Minutes Of Meeting) (need an example here). parser is responsible to read the document. top to bottom, left to right -> makes a tree-like structure. this tree is a big object.->called HTMLDOM. does  it again for css, the structure is called CSSdom. JS is not parsed, it is attached with a html element and tag.
OG NAME OF JS - mocha

cssOM and HTMLDOM combine together to form a resultant tree known as actualDOM(render tree). render tree is then parsed through layout tree(only visible tags). It is a full-fledged website. The loading of a website is done from top-to-bottom, left-to-right. This process is called painting of a UI. Also known as rendering. conciliation is the first loading/blinking of a website. Recurrence of these events is called re-rendering or reconciliation. Reconciliation was an issue, and react was introduced to solve that.

html-dom-tree(actualDOM/Render-tree), let's say an end node named "harsh", and I want it to change dynamically according to the user. it will require the entire website to reload just to show a single change.

JS is not parsed

JavaScript introduced mutli-thread using workers. it is async. no flow-break, multiple instance
Java garbage collection(mark & sweep)
1. getter(--proto) & setter {spread operator} Prototype (inheritance -SD2 interview)

let's visualize an UI with a navbar(main,home,about), sidebar, main, and footer. all its 1st reloads are denoted by N1, SB1, M1 & F1 (known as blinking of a page). when clicked on about us, the server will deal with it as a new request, only the content should be blinked to the page(home -> about), but the whole page blinks twice in this case. let's say an api has an image that costs $5 per reload, and every reload costs it . so to be cost effective, reactJS was introduced to stop reconciliation.

It was solved by creating a copy of actualDOM called virtualDOM(can't be printed) where changes are displayed. Both trees (actual and virtual) are compared using a diffing algorithm, and those changes are replaced, known as replacing a node. only the required changes will be blinking. it replaces the nodes in an optimized manner.
Critical thinking path

secondly react was made by facebook (now meta) to deal with the ghost messaging problem. [explain the ghost notification of facebook in brief] problem in state updation .reactJS hooks -> useState ->  bus service -> directly reflects changes

thirdly - SPA(Single Page Application). bunder . JSX -> babel (transfiler) -> converts into a format readable by the browser. bundler helps in component based development, making it easier to debug. Bundler wraps it around a thread and converts it into a single file which is referred to as a single page application.

seeing the potential, FB made React public (insert year) as a library, but it is used as a framework. Now it is used as a framework-cum-library.

JS is a popular language because of prototypal inheritance. that is why it can be used to write entire frameworks(api, backend, ...)

VCS

What is a version? (solution in an existing product)

1. carrot & 2 astrix. 

carrot(^) - 2.0.7 (7 is bug fixes, 0 is minor functionality change, 2 is entire codebase change. codebase change is restricted.)

2. astrix/universal(*) -> never used as it changes codebases 

Day 1

VCS pr-comparing 

Why is VCS needed? -> it provides branching (explain it). PR (pull-request), merge-conflicts, updating and rollback. registry(logs of commits, pr-comparing)

Git and github

Git is a CLI feature whereas Github is a GUI platform

Download git and nodejs
Setting up git hub

```
1. git config --global user.email “(email)”  
2. git config --global user.name “(name)”
3. git config --list
```

In vs code
```
git init
git add .
git status 
Staging Area
git commit -m “(message)”
git branch -M  main
git remote add origin [address]
git remote -v
git remote remove origin
git push -u origin main
git push -u origin main –force
```


works on master by default, but we use main 

also use https://docs.google.com/document/d/19ILAU7K9km2aqRB9HIeGeBZAVJxKCRNANSg-mOk-8Dg/edit?tab=t.0

Extensions for vs code
	1.HTML boilerplate
	2. Prettier
	3. Auto complete tag
	4. Auto rename tag
	5. Code runner
	6. Live preview
	7. Live server

explanation of a boiler plate code of html. definitions of tags, id, element & attributes

Typography
1. Headings - 
2. Paragraph, pre, anchor
3. Links
4. Image
5. Audio
6. Video
7. Lists (ordered & unordered)  

NOTE: HTML is a markup language

**Day 2**

VCS pr-comparing
Git and github
Git is a CLI feature whereas Github is a GUI platform  
Download git and nodejs  
Setting up git hub  

```
Git config –global user.email “(email)”
Git config –global user.name “(name)”
Git config –list    
```
In vs code  
```
git init
git add .
git status 
Staging Area
git commit -m “(message)”
git branch -M  main
git remote add origin [address]
git remote -v
git remote remove origin
git push -u origin main
git push -u origin main –force
```
  
**Extensions for vs code**  
1.HTML boilerplate
2 Prettier
3.Auto complete tag
4.Auto rename tag
5.Code runner
6.Live preview
7.Live server
  
**Typography**  
1. Headings 
2. Paragraph
3. Links
4. Image
5. Audio
6. Video
7. Lists (ordered & unordered)  

h/w
1. Name
2. Bio
3. Skills i have (using lists)
4. Skills to acquire(using lists)
(done)

**Day 3**  
1. Definition list - dt/dd (also introduced to ayra-accessibility tech)
2. Formatting tags(bold, strong, highlighted, italic, underlined, striked,superscript,subscript,mark,delete,insert,small,sample,qoute)  
3. Tables (table tag, thead-> tr,td,th, tbody, tfooter, border attribute,  (task was given to make a time table which i did already)
4. Symantec Tags/non symantec tags & inline block
5. Input (type, name, id, placeholder, select(dropdown) option attribute fieldset, legend)
6. Forms(collection of input)/ json (get & post)  
Attributes - action(after submit) and method(data handling). Get method for request on browser. To send data use a form.  
get(available for public, default) .post(encrypted)  
  
H/W: 1. Make an event registration form(let’s say a concert) input using a div , input dropdown(inhouse/outside ,type of ticket add an image a nav bar) ( done)
1. Portfolio using all topics in a structured way (done)  
Note: 1.always follow a what-when-how in every topic.  
          2.Post periodically in public (linked in) to showcase what I'm learning. Consistency is the key. ( I hesitate while posting, so we’ll design the posts in a way that I feel confident before posting it, only posting what’s absolutely necessary)  
  
  
DAY 04
  1. Tag vs Element -> Element = Tag + attribute
  2. Inline vs Block
  3. Aria-label - read aloud (ex - <span

  role="checkbox"

  aria-checked="false"

  tabindex="0"

  aria-labelledby="tac"></span>
<span id="tac">I agree to the Terms and Conditions.</span>

)

4. CSS - Cascading Style Sheets  
Cascading means style overriding (interview)  
Types -  1. Inline, 2. Internal, 3.External  
  
Inline: within the line  
Internal: ID(style tag in head) (call by id, name ,tag,attribute) (refer code for more notes)
Priority:  inline>ID>CLASS> Attribute/Tag   
External  
  
NOTE: in context of internal and external, the style that is applied later is prioritized.

4. Box-model    
5. * property
6. Width, padding, border( I always get confused in this)  
    Space between content and border is padding.
7. Spacing:1. top-bottom/left-right  
      2 top-right/ bottom-left.
8. Specificity: px( 1.physical unit = 0.26mm, pre-defind on root  
    1. Don’t make horizontal scrollable UI, means don’t use px while defining dimensions.  
    2. Em - depends upon font-size of parents, if not defined then on root’s font-size (drawbacks - ambiguity,, only use when all elements are of same type)  
    3. Rem (depends directly on the root)  
    4. %  (depends on parent)  
    5. Viewport (viewport(visible) [depends on root] vs screen(entire/not visible))  
Interview questions:  
9. Box-Model:
I. content-width
Ii.padding ( 1. top,bottom, 2. left, right 3. ) (ex-  padding: 10px 20px 30px 50px;
)
Iii. border (1. Border-width, 2.border-color, 3.border-style (using them together and separately) 4. border -radius -
Iv. margin (top,bottom, left, right)  
  
  
TASK:  
Biodata- 1. Intro (rounded from top left = 20px, 5px padding)  
	      2. Skills (rounded from top right =20px, 5px padding)
	3. Hobbies (rounded from top, flat bottom)

NOTE: remind me to rewatch the lecture as i didn’t fully get it.  (done)
  
**DAY 05:**  
1. Important key word in css  
2. id-# class-. (id vs class)

3.DRY  
4. Sibling selectors  
5. Nth selectors
6. Attribute selectors(input[type='text'], input::placeholder)
7. Sudo selectors (hover, before, after

to-do(add colors to biodata)

****DAY 06**
task-
four boxes
1. 1200px x 800px
2.  50% of first
3.  30% of second
4.  20% of third (done)
   
   complete assignment 1 ( pending)
**Fonts**- how text will look
properties:
	1.font-family( font-size,style, weight, family{browser dependent, font stacking} )
	2. third-party font-borrowing (import, embedded code/CDN)
Texts{text-align, transform, text-decoration, text indent, letter spacing, word-spacing, text shadow}

use these properties on portfolio(waiting, since missed a few lectures and this will be given on daily basis, so will do it once i completed the backlog. plus you can help me design it using all the necessary things to make it perfect)
5. filters for image. properties:
   (i) blur - % (ii) sepia (iii) greyscale (iv) opacity (v) hue rotate (vi) invert
**BOX model** :- every element and every tag used to build a website is a box. it is divided into four parts.
(i) content - innermost part
(ii) padding - ( imma need u to define them , Gemini its confusing) - between content and border
(iii) border - between padding and margin
(iv) margin - outermost
( include their syntaxes too)
NOTE: margin is not a part of box-model
Q. Why is box model needed?
A. (something like the defined size is less than that is being displayed. i didn't fully get it)

**Box-Sizing**
1.content box(by default): additional will be added to page's 50px approx.  (first prioirty is content) 
here, total height = content height + padding top +padding bottom +border bottom + border top, and
total width = content width + padding left + padding right + border left + border right

2.border-box(prioritize):  everything is between the defined area.( border is prioritized, content is least)
here, total h = bt + bb + pt + pb + content
total w = bl + br + pl + pr + content

NOTE: 1. most important topic. use it in the cv
2. universal css:
```
*{
 margin: 0;
 padding: 0;
 box-sizing: border-box;
}
```
   
IMPORTANT:
 flexbox (flexible-box):  to move a content, its parent must be larger than the content itself.
 it has two parts. flex-container & flex-child. display flex makes the container flexible, allowing children to move freely. 
 
 flexible box axis system ( will be needing a diagram)
  (i) main-axis(x)  (ii) cross-axis(y)
  
  in row-nature alignment, main axis is x-axis and cross-axis is y, whereas in a column nature alignment main axis is y-axis and cross axis is x-axis.
 both main-axis and cross axis have different properties
justify - always on main axis; align- always on cross axis(most important)

my note: to center a div horizontally: 
```
display:flex, 
flex-direction:row  
justify: center; 
align: center
```

to center a div vertically:
```
display:flex,
flex-direction:column,
justify-content: center;
align: center
```


My note: at the end, guide me on how to implement these things, so i can remember them by heart.

to do- assignment 01


**Day 07**
1. Justify content:  centers on main axis and align center on cross axis.
Properties on parents :
(i) flex-start: Default value. Items are positioned at the beginning of the container
(ii) flex-end: Items are positioned at the end of the container
(iii) space-around: Items will have space before, between, and after them
(iv) space-between: Items will have space between them
(v) space-evenly: Items will have equal space around them

if the dimensions pf the container is less than that of items they will shrink. to avoid that, we use wrap
(i) wrap
(ii) wrap-reverse
(iii) no-wrap (default) 
 my Note( these are most important and i know i'll forget them. focus on them )
 
 Properties on child:
 (i) flex-grow : specifies how much the item will grow relative to the rest of the flexible items inside the same container
syntax: flex-grow: 2; (ratio)
 (ii) flex-shrink (define it)
 (iii) flex-basis: explicitly manipulate a child's width/height
 (iv) align-self: adjusts itself accordingly
 (v) order: defines arrangement, can be given negative values too.
 task: combine box-model and flexbox to create a this, give each inside box a different color. (done)
 ![[Pasted image 20250902134232.png]]
**GRID** : divides into rows and columns, used to create a complex layout. track, grid-area 
(i) grid-template [ dimension-column  dimension row]
  snippet: grid-template-columns: repeat(3, 100px);

Fractional unit (define it) (used to make responsive layout)
snippet:  grid-template-columns: repeat(3, 1fr);

grid-row-gap, grid-column-gap

by default positions are stretch. 

justify/align items (for individual items). justify/align content (for entire grids)

**building a layout**
properties to move/resize the elements within a layout (use dev tools to check the number that is to be given)
(i) grid-column-start:  grid-column-start: 1;
(ii) grid-column-end:    grid-column-end: 4;
(iii) grid-row-start 
(iv) grid-row-end

home work (i)design these. (done)
![[Pasted image 20250902154853.png]]
(done)
(ii) complete-flexbox froggy (done)


**Day08**

grid-template areas, grid template columns


task: create:
![[Pasted image 20250907123844.png]]

CSS positions:
orthodox and unorthodox positons/ dimensioning system
	1. Static (default) - (immovable no tblr)
	2. relative - remains in document flow, movable from its current position, leaves footprint (tblr flexibilty), space is preserved
	3. absolute - leaves document flow, movable from current position, (use case  when aligning a nested div, parent-  relative, child absolute. z-index can be used to modify stacking )
	4. fixed - immovable, out of doc-flow (used for adverts)
	5. sticky - mixture of relative and fixed (nav -bar)

![[Pasted image 20250908021237.png]]


**Responsive Web Design**

media query (instruction)
Note: bootstrap gives 87% responsiveness by default. no end-to-end responsiveness. for near perfect(93%-97%) use tailwind. for full flagged, use media-query
media-query violates DRY principle. it uses breakpoints, acts like a conditional statement, increases complexity, decreases readability, that's the reason we don't use it. (media query is depricated)

Two types:
1. height/width(min/max height, min/max width)
		Note:  breakpoints for width: (i) 978px (ii) 576px (iii) 376px {always define these for media query: Tablet, Mobile, feature-phone}
2. .orientation(portrait/landscape)


**DAY 09**
 for responsiveness:
Advanced breakpoints:
1. 976 - 978px 
2. 576-578px
3. 374-376pc
Normal breakpoints
	1.potrait
	2. landscape


Keyframes: are properties at a particular point of time (generally used at 0%, 50% & 100%)
		to make it smooth, we break it down at (0% , 25%, 50%, 75% and 100%)
		as the number of breakpoints increases, smoothness of animation increases
animation:

properties. animation's name, animation duration, animation flow (can  be combined like margin)
Animation : [name], [duration], [timing function] [Iteration Count] [Direction]

task: make a submit button (done)
initial: size: 10px 20px color yellow
after:  size: 20px 40px color green


BOOTSTRAP :
CDN(Content Delivery Network)(API/URL/Link) -> Gateway
when bootstrap is connected, we have to only include keywords in classes and the property will be fetched from backend via CDN
ex- instead of defining  background color: red, in css, we can define "bg-danger" as class name, through CDN, bg color will be defined as red.
custom knowledge of css is required to work with bootstrap
WHY BOOTSTRAP? - to make a website responsive, without defining breakpoints
CONS: only 87% responsiveness
PROS:(i) breakpoints: small(sm), medium(m), large(l), XL, XXL
	to attach it, we'll go the bootstrap's website
(ii) No writing to codes, just copying and customizing
refer bootstraps docs , install bootstarp5 extension

bootstrap-containers. container-fluid
snippet:
 .container (creates a responsive container with margin padding, height-width, )
 .container-sm, md, lg, xl ,xxl ,fluid
breakpoints -sm, md, lg, xl ,xxl ,fluid,(media query) 
NOTE: everything in bootstrap must be inside a container.

TYPOGRAPHY
1. heading (heading) :heading
2. p (same as HTML)
3.  display(better heading)
4. mark
5. small
6. underline
7. colors {danger(red), success(green) warning(yellow), primary(blue) , secondary(grey), info (cyan) ,text(color)}
8. image {fluid, thumbnail, float(align) }
9. table (table, table-border, table-hover, table-border, table-responsive)
10. table-row(tr class="table-dark", table-info, table-secondary ,table-primary, )
11. mt5(pointers, margin-top),d-flex(display-flex)
12. justify-content-center align-items-center
13. buttons(danger, warning, info, success, secondary, light,dark, link, block, btn-group)
14. card(card-head, card-body, card-footer)

to include external css in bootstrap, give a class name and use style tag
TASK - time table (done)

assignment 1 - to be made again as it was i ecommerce website not an restaurant (we'll use Bootstrap this time) (not done)

**DAY 10**
	15. Alerts (uses js, how to use js in bootstrap, defer keyword
	    <script defer src="https://cdn.jsdelivr.net/npm/bootstrap@5.0.2/dist/js/bootstrap.bundle.min.js" integrity="sha384-MrcW6ZMFYlzcLA8Nl+NtUVF0sA7MsXsP1UyJoMp4YLEuNSfAP+JcXn/tWtIaxVXM" crossorigin="anonymous"></script>)

note: while building a website from bootstrap, i just need to copy the elements from the site and customize them according to my need

16. role(aria-tags)
17. anchor
18. dismiss tag(imp) - uses a predefined js class , databsdismiss
19. Forms ( class="form-label"  and class="form-control" , disabled-attribute , value-attribute, bootstarp-range, date, readonly, readonlyplaintext, file control, color picker, floating, text- area, form-check label)
20. pagination, spinners
21. switch
22. modal (used for collapse and forms) and Accordion
23. nav-bar(navbar navbar-expand-lg navbar-dark bg-dark, expand/collapse , cross-referencing)
24. toggle, target
	    
	    
	NOTE: explicitly said to use these components in projects, explicitly said in lectures" why are u writing, just copy and modify according to need, 3 important components. form card and nav-bar
	
	
	Task event registration using bootstrap(in class work, done)
	to do: travel website in bootstrap
	
	MY note: didn't do much on this day just skimmed through the video as was covering up the backlog
	
	to add the travel website on linkedin, with recorded working
	 always use nav-bar collapse
	
	also, after this aws cloud practitioner after/during mern



**DAY 11**

		1. grid (even when it is responsive, it'll try to shrink after 12th column, 12 is the limit in a row)(properties, col-1,2,3... col bg-primary....)
		2. nested-grid: column inside a column\
		3. grid option - (extra small(xs), small(s), madium(m), large(l),extra large(xl), extra extra large(xxl) )


to-do(home-work , not done) :
	photo-flex (gallery)
	 travel website(we were given options between css and bootstap, i'll go for bootstrap as already done one via css. explore the mountain with us.) (ongoing)


**DAY 12** (intro to JS)
1. What makes a language a programming language?
   JS is called the soul of web-dev. developed in 1995 , initially named mocha(this was a question that decided t-shirt in workshop).
2. why we prefer it? -> mocha's basic goal was to be a script for CLI 
3.  function -> write one time, use anywhere _
4. mocha changed its name to javascript, just beacuse java was trending. JS is popular than Java because
   
   JS defination - a synchronus, single thread promgramming language. it's also a dynamic type, loosely type, flexible and agile
		Drawbacks: 
(i)  let's say there were three files with different download time, synchronous nature was holding it back. fix- async tasks were introduced
(ii). single-threaded,, else languages were multi-threaded by default. fix -  workers were introduce, small spaces were introduced, divided tasks into multiple parts, reducing waiting queue, which acted like multi thread
(iii). Garbage collection - mark and sweep algo was introduced, it watched the call-stack, it removes a task as soon as it is executed, but they could be used again 

  1. prototypal behavior (never quitting attitude -> prototypal behavior, moves in hierarchy)
  2. Global Window Object (this(global pointer) and window(global object) are same, but different execution)
  3. getter and setter
  4. callstack _last in first out;
  5. web apis - microtask queue( job queue) / macrotask queue  ( task queue)
  6. event loop (soul of runtime environment, never ending loop, keeps callstack running)
![[Pasted image 20250912010046.png]]
		

call stack (lifo) -> function -> event loop -> mark and sweep -> empty playground(anonymous) -> web-apis via third party

macro - low priority task
micro - high priority (functions
combination is called callback queue
interview- 
 prototypal behavior - behavior where it never quits
 Q, define prototypal inheritance (SD-2 level)
priority: micro -> macro ->
 
how does JS run? -> it uses nodeJS 

-> AST (Abstract Syntax Tree) -> interpret  (till 2005)

JS is also parsed. JIT (just in time programming) -> watcher(only when complex) -> interpreter

NOTE: (i) JS waits for none
	   (ii) everything in web-dev ends on  an object
	   (iii) shortest program in js is null


**DAY 13**
JS
1. memory management: (Parenthesis/primitive(stack) and reference/(non-primitive)(heap/array) - random memory allocation, pushes a copy to stack) (shallow copy and deep copy problem - changes made on object 2 are directly reflected on object 1)
2. GEC(how JS runs your program): Global Execution Program (Important for guess the output of a program type questions in round 1 of interviews)
   
second step: Thread execution
(1) memory allocation (2) code execution
use these snippet to define these processes

```
var a = 10; 
function double(num) {
return num = 2; 
}
var res = double(6);
console.log(res);
var res1 = double(a);
console.log(res1); (ask me to upload its screenshot)

```
anonymous function
var, let, const keywords

hoisting - (will need u to define it along with hoisting processes in var ,let, and const  
what i get, var can be initialized even before declaring its value)

TASK: find the output of the program
	// try to guess the output
```
let a = 10;
const b = 20;
function a() {
    console.log(a);
    let c = 30;
    console.log(c);
}
a();
console.log(a);
var c =40;

// output will be: (an error. explain why)
// 10
// 30
// 10

```
**datatypes**
 typeof (function) is used to check datatype
 (i) Primitive
1. var
2. let
3. bool
4. bigint
5. number
(ii) Non-primitive/refernce:
	1. object: key-value pair
	2. null (type tag is object):
	3. undefined


NOTE: Global error/ambiguity: Null is an object (for interview)
		null(var isn't declared) vs undefined(var is declared, no value assigned)
		
		datatype notes:"https://docs.google.com/document/d/1qYMb06vn5s13t1RLK2pITKhjd2LWb_yhv72Cppg9JCY/edit?tab=t.0"
		
		repo for js https://github.com/sudheerj/javascript-interview-questions" (use for each topic, only top 100 questions)


{include everything, i've only noted things what i've been told is important}
function, fat arrow function

day14
iffe(used on the spot) -> fixes global variable pollution(unused varible warning, use and throw programming, used in modular programming)

	1.tree-shaking algo/dead code algo - removing the code that has no effect. -> function borrowing
	types of function: named, anonymous, iife, arrow

	function has two parts:
		(i) defination
		(ii) calling
	NOTE: Function is a first class citizen. they carry different instance, even if they share the same name
	2. conditions : (if/else/switch)
	3. operators : 
	4. iteration(loops)
	5. switch
	6. deep/shallow copy 
	   
	   to do: JS switch questions
	
day15
	7. rust args(multiple argument handling)/ layer-wise de-structuring of API
	8. spreading an argument/ rust parameter
	9. scoping (global, function and block)
	    reference error, block scope (var is a function-scoped), local, lexical(hierarchal) environment scoping, scope-chaining
	5.closure(very imp): (phenomena) combination of a function & lexical environment within which the function was declared, it creates an instance, which bypasses mark and sweep (GEC is must in this type of problem, do the GEC on paper)
	10. callback function - passed as an argument inside another function, that can be called later, used for async programming. functions that recieve a callback function are known as higher-order function.
	 11. idea-feasibility (ex- ordering an article)
	 12. IOC (Inversion Of Control) 
		(modular programming approach - to check if each function in heirarchy is working correctly)
		problem 1: passing function, if an function doesn't run in its intented manner, the entire layout collapses, forming a callback-hell (used example- cooking noodles)
	13. Pyramid of doom - callback-hell, it is a complex structure that is difficult to read, analyze and debug, FIX: Attaching of function
	14. attaching a function (promises) {just the intro and requirement} - every async task returns a promise, initializing a promise initiates a promise state, two cases - (i) fulfilled (ii) rejected -> in either case, output is recieved. when fulfilled use *.then* when rejected use .catch -> .finally (end of task)
	15. typeofFunction
	16. immediate invoke function expression (iffe)
	
	for interview: define scope-chaining.(parent and child are bound together, these boundings are known as closure) closure ( 2-button chain-problem ) . implementation of closure
	how to write an HOF (array.prototype)
	    
	note: didn't get rust args, useful for apis


**DAY16**
task - make a 4 step sandwich maker, 5 sec time using callback
11. HOF, map (how to make a higher-order function) -> (.prototype)

**DAY17**
12.  promise
13. currying - parsing each argument as a function
14. DOM (Document Object Model)
15. BOM (Browser Object Model) {this and window in browser's console}
16. Call(once), bind(frequent) and apply(more than one buy not frequent){} (function borrowing)} 
17. instance is given to a method, if a single function is defined with two names, it will be treated as a different function
18. call example, asking for bike from a friend, owner doesn't allow pillion, aka multiple arguments)
19. apply (allows pillion, aka multiple arguments)
20. bind (independent, can follow and rule, comma and or treated as different function.)
21. browser inspect -> 

note: UX is always prioritized 

Task order booking 7 step using HOF ( to do again. i copied it from gpt)

JS is written below the html, because it is important to get the structure ready before it's functionality. 
Markdown language

question for next class - node list vs array list vs html collection (class list)
					inner html vs text content
					dom vs bom
**DAY18**
didn't take class, yet event delegation
append, create
events(imp)
eventlistener (name of event, callback function, )
event.target

interview - 
**DAY 19**


**DAY20**
async -> multiple tasks at a time
(i) setTimeout (ii) set
JS conference channel -> eventloop JS conf -> loupe js(visualizer)

For interview -> async nature comes due to nodeJS

**DAY21**
1. Local storage vs session storage (refer GFG's site difference table)
2.  Optimization techniques : debouncing and throttle
	ex-request-response cycle with minimum delay breaks if something is changed(debouncing-> interval )
		throttle -> limits the rate leading to  resource efficiency -> ex- yt live stream chat
			it needs last call and current call. if difference is equal to greater than the interval, it is allowed, else it is rejected
			(define , use-case, and implementation)
3. load balancer : smartly manages the resource to maintain the requests. first : uses - round robin. second : waited-round-robin third: least connection(explain these algos)


JS is done(idk shit)

**REACT :**
![[Pasted image 20250925094402.png]] Node JS environment

when writing server-side scripting, we borrowed some functionalities of C++ called livuv.
to manage OS -> module(piece of code that that solves a problem)
module , fs module, os-module, path-module, npm

npm(node package manager)
ex - carrot-versioning of a package

HOW IS A NODE APPLICATION MADE?
node --watch index.js
gitignore - contains node module, used to remove the node packages, to reduce the size of project while uploading
react - doesn't own anything. framework cuz it has everything, library cuz borrows everything.

figlet package
import figlet from 'figlet'

task: TTS coverter