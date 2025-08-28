**

day 0, web basics

1. networking
2. client server architecture
3. example of ordering a meal and comparing it to client-server architecture.
4. Each time you make a request, you get a response. Not getting a response is also a response
5.  client (front-end) is connected to backend via a bridge(API), driver to connect to database with backend (client-server architecture)
	establishing connecting, between client server, TCP(acknowledgement at every step, end-to-end encryption, hard to hack) vs UDP(no acknowledgement, no encryption, easy to hack)

6. What do we get in response? -> internet is connected in wires -> data travels to packets -> let's say those are html,css,js -> merged by "BROWSER" using PARSERS (need an example here). parser is responsible to read the document. top to bottom, left to right -> makes a tree-like structure ->called HTMLDOM. does  it again for css, the structure is called CSSdom. JS is not parsed, it is attached with a html element and tag.

cssDOM and HTMLDOM combine together to form a resultant tree known as actualDOM(render tree). render tree is then parsed through layout tree(only visible tags). It is a full-fledged website. The loading of a website is done from top-to-bottom, left-to-right. This process is called painting of a UI. Also known as rendering. conciliation is the first loading/blinking of a website. Recurrence of these events is called re-rendering or reconciliation. Reconciliation was an issue, and react was introduced to solve that.

html-dom-tree(actualDOM), let's say an end node named "harsh", and I want it to change dynamically according to the user. it will require the entire website to reload just to show a single change.

let's visualize an UI with a navbar(main,home,about), sidebar, main, and footer. all its 1st reloads are denoted by N1, SB1, M1 & F1 (known as blinking of a page). when clicked on about us, the server will deal with it as a new request, only the content should be blinked to the page(home -> about), but the whole page blinks twice in this case. let's say an api has an image that costs $5 per reload, and every reload costs it . so to be cost effective, reactJS was introduced to stop reconciliation.

It was solved by creating a copy of actualDOM called virtualDOM(can't be printed) where changes are displayed. Both trees (actual and virtual) are compared using a diffing algorithm, and those changes are replaced, known as replacing a node. only the required changes will be blinking. it replaces the nodes in an optimized manner.

secondly react was made by facebook (now meta) to deal with the ghost messaging problem. [explain the ghost notification of facebook in brief] problem in state updation .reactJS hooks -> useState ->  bus service -> directly reflects changes

thirdly - SPA(Single Page Application). bunder . JSX -> babel (transfiler) -> converts into a format readable by the browser. bundler helps in component based development, making it easier to debug. Bundler wraps it around a thread and converts it into a single file which is referred to as a single page application.

seeing the potential, FB made React public (insert year) as a library, but it is used as a framework. Now it is used as a framework-cum-library.

JS is a popular language because of prototypal inheritance. that is why it can be used to write entire frameworks(api, backend, ...)

VCS

What is a version? (solution in an existing product)

1. carrot & 2 astrix. 

carrot(^) - 2.0.7 (7 is bug fixes, 0 is minor functionality change, 2 is entire codebase change. codebase change is restricted.)

2. astrix/universal(*) -> never used as it changes codebases  →  

Day 1

VCS pr-comparing 

Why is VCS needed? -> it provides branching (explain it). PR (pull-request), merge-conflicts, updating and rollback. registry(logs of commits, pr-comparing)

Git and github

Git is a CLI feature whereas Github is a GUI platform

Download git and nodejs
Setting up git hub
1. git config --global user.email “(email)”  
2. git config --global user.name “(name)”
3. git config --list

In vs code

(i) git init
(ii) git add .
git status 
(iii) Staging Area
(iv) git commit -m “(message)”
(v) git branch -M  main
(vi) git remote add origin [address]
(vii) git remote -v
(viii) git remote remove origin
(ix) git push -u origin main
(x) git push -u origin main –force

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
1. Git config –global user.email “(email)”
2. Git config –global user.name “(name)”
3. Git config –list  
  
In vs code  
(i) Git init  
(ii) Git add . 
Git status  
(iii) Staging Area  
(iv) git commit -m “(message)”
(v) git branch -M  main
(vi) git remote add origin [address]
(vii) git remote -v  
(viii) git remote remove origin  
(ix) git push -u origin main
(x) git push -u origin main –force  
  
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
*{
 margin: 0;
 padding: 0;
 box-sizing: border-box;
}
   
IMPORTANT:
 flexbox (flexible-box):  to move a content, its parent must be larger than the content itself.
 it has two parts. flex-container & flex-child. display flex makes the container flexible, allowing children to move freely. 
 
 flexible box axis system ( will be needing a diagram)
  (i) main-axis(x)  (ii) cross-axis(y)
  
  in row-nature alignment, main axis is x-axis and cross-axis is y, whereas in a column nature alignment main axis is y-axis and cross axis is x-axis.
 both main-axis and cross axis have different properties
justify - always on main axis; align- always on cross axis(most important)

my note: to center a div horizontally: display:flex, flex-direction:row  justify: center; align: center
to center a div vertically: display:flex, flex-direction:column  justify: center; align: center

My note: at the end, guide me on how to implement these things, so i can remember them by heart.

to do- assignment 01