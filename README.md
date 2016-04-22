Front-end Job Interview Questions
This file contains a number of front-end interview questions that can be used when vetting potential candidates. It is by no means recommended to use every single question here on the same candidate (that would take hours). Choosing a few items from this list should help you vet the intended skills you require.
Note: Keep in mind that many of these questions are open-ended and could lead to interesting discussions that tell you more about the person's capabilities than a straight answer would.
Table of Contents
1	General Questions
2	HTML Questions
3	CSS Questions
4	JS Questions
5	Testing Questions
6	Performance Questions
7	Network Questions
8	Coding Questions
9	Fun Questions
Getting Involved
1	Contributors
2	How to Contribute
3	License
General Questions:
1: What did you learn yesterday/this week?
A: Learning AngularJS.

2: What excites or interests you about coding?
A: Cool. Reduce the boring & repeating works. The learning process is happiness

3: What is a recent technical challenge you experienced and how did you solve it? - What did you contribute?
A: My technology is old. I have to learn new technology and refresh JavaScript skill.
I have to contribute more time.

4: What UI, Security, Performance, SEO, Maintainability or Technology considerations do you make while building a web application or site?
•	A: UI:
o	Constraint vs Freedom: How much do you let the user do (guided wizard vs adobe photoshop-like app)
o	Direct on-canvas vs form-based editing
o	Navigation and progress tracking (e.g. step 1 of 5 done)
o	links: 1, 2
•	Security:
o	User authentication
o	Server authentication
o	Is RBAC (Role Based Access Controls) needed
o	Secure transmission (SSL)
o	Firewalls
o	Validate user input
o	What access does the user have to your data
o	links: 1, 2
•	Performance
o	Number/size of external resources
o	Optimize images
o	Optimize code
o	Placement of script blocks
o	Minimize cookie size, eliminate dead cookies
o	Low-bandwidth options
o	links 1, 2, 3, 4
•	SEO
o	Content on your page relevant to your targeted keywords
o	Title, meta-description, meta-keywords, h1 - content rich
o	Pretty url’s
o	Use of 301 redirects
o	Get rid of 404’s, 500’s,
o	links: 1, 2, 3, 4
•	Maintainability
o	Very tight, issue specific commits
o	Helpful commenting
o	Informative use of Github tools - issues, PR’s, milestones
o	links: 1, 2
•	Technology
o	What browsers, devices, screen resolutions should you be targeting

5: Talk about your preferred development environment.
A: win/Unix(Mac OS), sublime text 2/3, Visual studio/vi, Chrome/Firefox/IE9 and browsers devTools/git/node

6: Which version control systems are you familiar with?
A: CVS (Concurrent Version System) and Subversion.

7: Can you describe your workflow when you create a web page?
A: Study prototype. Set structures(html tag). Render with style. Add interactive by script.

8: If you have 5 different stylesheets, how would you best integrate them into the site?
A: You DON'T. Multiple CSS always lead to redefinition of classes and errors. 
A class can be named the same way in different CSS files, and the cascading will lead to the last definition being applied! 
Say you have 
body {background-color: blue} in sheet 1 
and 
body {background-color: red} in sheet 2 
If you include then in that order, the bkg will be red. 
The other order will be blue. 
JOIN all your CSS in ONE sheet, check for duplicates, eliminate conflicts.

9: Can you describe the difference between progressive enhancement and graceful degradation?
A: Bonus points for describing feature detection
Graceful degradation:
Providing an alternative version of your functionality or making the user aware of shortcomings of a product as a safety measure to ensure that the product is usable.
Progressive enhancement:
Starting with a baseline of usable functionality, then increasing the richness of the user experience step by step by testing for support for enhancements before applying them.

I agree with progressive enhancement, and increasing user experience with feature detection. For example, once I detected that the browser support round-corner or shadow text, I will apply the futures to pages.

10: How would you optimize a website's assets/resources?
A: Looking for a number of solutions which can include: File concatenation, File minification, CDN Hosted and Caching.

11: How many resources will a browser download from a given domain at a time?
What are the exceptions?
A: IE7 allowed only two concurrent connections per host. But most browsers today allow more than that. IE8 allows 6 concurrent connections, Chrome allows 6, and Firefox allows 8.
So if your web page only has 6 images, for example, then it'd really be pointless to spread your images across multiple subdomains.

11: Name 3 ways to decrease page load (perceived or actual load time). resource1 resource2 resource3
a.	gzip
b.	cache
c.	minify js/css	(resource2- Second, minimize HTTP requests. Rather than forcing your site to request multiple files for images, content or ads, combine some pages.)
d.	optimize images 	(resource1- First, optimize, optimize, optimize. Check the types of images you are using on-site and ensure the file format is appropriate.)
e.	cdn		(resource3- Finally, resize elements before they are uploaded into the HTML.)

12: If you jumped on a project and they used tabs and you used spaces, what would you do?
A: Suggest the project utilize something like EditorConfig (http://editorconfig.org), Conform to the conventions (stay consistent), issue: retab! Command (sublime text retab setting).

13: Describe how you would create a simple slideshow page.
A: http://brianshim.com/webtricks/add-a-slide-show-to-your-website-the-jquery-way/
 <!-- Cycle - "slideshow" plug-in -->
<script type="text/javascript" src="scripts/jquery.cycle.all.js"></script>

14: If you could master one technology this year, what would it be?
A: Ruby on Rails. For a good job.

15: Explain the importance of standards and standards bodies.
A:
16: What is Flash of Unstyled Content? How do you avoid FOUC? answer
A: FOUC meaning flash of unstyled content.
minimizing FOUC by hiding all or part of the web page until all styles and JavaScript are finished by applying a class name "js" as the selector that hides all content within a container that has an id="fouc". The "fouc" element is unhidden using a JavaScript getElementById function setting the display value to "block" level.

17: Explain what ARIA and screenreaders are, and how to make a website accessible. answer
A: Accessible Rich Internet Applications (ARIA) defines ways to make Web content and Web applications (especially those developed with Ajax and JavaScript) more accessible to people with disabilities. For example, ARIA enables accessible navigation landmarks, JavaScript widgets, form hints and error messages, live content updates, and more.

18: Explain some of the pros and cons for CSS animations versus JavaScript animations. not an answer answer
A: Use CSS when you have smaller, self-contained states for UI elements. Use JavaScript when you need significant control over your animations.

19: What does CORS stand for and what issue does it address? answer
A: CORS can be used as a modern alternative to the JSONP pattern. While JSONP supports only the GET request method, CORS also supports other types of HTTP requests. Using CORS enables a web programmer to use regular XMLHttpRequest, which supports better error handling than JSONP. On the other hand, JSONP works on legacy browsers which predate CORS support. CORS is supported by most modern web browsers. Also, while JSONP can cause cross-site scripting (XSS) issues where the external site is compromised, CORS allows websites to manually parse responses to ensure security.[

HTML Questions:
20: What does a doctype do?
A: A DOCTYPE is a required preamble. DOCTYPEs are required for legacy reasons. When omitted, browsers tend to use a different rendering mode that is incompatible with some specifications. Including the DOCTYPE in a document ensures that the browser makes a best-effort attempt at following the relevant specifications.
21: What's the difference between standards mode and quirks mode? answer
A: There are now three modes used by the layout engines in web browsers: quirks mode, almost standards mode, and full standards mode. In quirks mode, layout emulates nonstandard behavior in Navigator 4 and Internet Explorer 5. This is essential in order to support websites that were built before the widespread adoption of web standards. In full standards mode, the behavior is (hopefully) the behavior described by the HTML and CSS specifications. In almost standards mode, there are only a very small number of quirks implemented.

22: What's the difference between HTML and XHTML?
A: Comparing HTML(Hypertext Markup Language) and XHTML(Extensible HTML) could be like comparing identical twins since there are only a few minor points which we can actually point out as being different. This is due to the fact that XHTML was derived from HTML just to conform with XML standards. The primary major difference between the two is the relative strictness of XHTML compared to HTML. While someone coding in HTML could get away with some lapses in structure and coding, that is no longer possible with XHTML. The need to come up with XHTML emerged from the fact that HTML has become to convoluted with browser specific tags that pages coded in html doesn’t always look the same in all browsers.
All XHTML documents must have only one root element and all elements must be written in lowercase, closed, and properly nested. And although you can actually do the same with HTML, it is actually not required and you can violate any or all of those rules and your HTML document can still be opened without any errors. Another XHTML only requirement is the declaration of the DOCTYPE that determines what rules your document would follow; which it inherited from XML. Not only is the strictness of XHTML prominent in the structure, even variables have been limited to lower case letters and the values assigned to them must be surrounded by quotation marks for it to be properly recognized.


23: Are there any problems with serving pages as application/xhtml+xml?
A: It's nearly a decade since W3C produced the first XHTML standard. In all that time, very few sites adopting it have gone as far as to serve the preferred MIME type (application/xhtml+xml). This is because it has been difficult to do well, and text/html sort-of works, so most website administrators don't bother.
There are two broad approaches used to change the MIME type:
	*Use one of Apache's features to detect the browser's capability
*Use server-side scripting - typically PHP - to detect the browser's capability

24: How do you serve a page with content in multiple languages?
A: To serve a page with content in multiple languages, there are four steps:
1. You must have translated/localized pages on the server for each language you intend to support.
2. Your server must recognize the browser’s language request.
3. You must carefully name the files for the localized pages, so the server has a systematic way of locating them.
4. You need a method for serving a generic page when you don’t have the requested language.

25: What kind of things must you be wary of when design or developing for multilingual sites?
A: <HTML lang=" "> tag is where you need to manipulate using php...so that it changes to the language the server you are surfing from.for instance:
<?php if(strstr($_SERVER['REQUEST_URI'],'/nl/')){echo("<html lang=\"nl\">" ;
?>
26: What are data- attributes good for? answer
A: You can store some extra information that doesn’t have any visual representation.
The W3C specification for data-attributes states that:
Custom data attributes are intended to store custom data private to the page or application, for which there are no more appropriate attributes or elements.
Custom data- attributes are a great way to simplify the storage of application data in your web pages.

27: Consider HTML5 as an open web platform. What are the building blocks of HTML5? answer
A: more semantic text markup, new form elements, vedio and audio,new javascript API, canvas and SVG, new communication API, geolocation API, web worker API and new data storage

28: Describe the difference between a cookie, sessionStorage and localStorage.
A: Now there are such way to keep data on front-end side.
•	HTML5 web storage
o	HTML5 local Storage
o	HTML5 session storage
o	HTML5 web database
•	Cookies
localStorage - stores data with no expiration date sessionStorage - stores data for one session
•	HTML5 web storage = generic umbrella term for the new client-side data storage options:
o	Web Storage is more secure and faster. The data is not included with every server request, but used ONLY when asked for. It is also possible to store large amounts of data, without affecting the website's performance.
o	Local Storage = persistant and scoped to the domain(store data with no expiration date). At the moment two flavors are usually mentioned:
o	'default' = stores things in name/value pairs
o	Web SQL (aka Web Database) = uses a SQL database
o	Session Storage = non persistent and scoped only to the current window(stores data for one session)
•	Cookies = the old school way of doing all of the above. Stores name/value pairs per domain.

29: Describe the difference between <script>, <script async> and <script defer>. answer1 answer2
A:  <script src="myfile.js"></script>
When the browser comes across the above line in your markup, this is what happens.
1.	Pause pars¬ing the document.
2.	Make a request to fetch the file.
3.	Exe¬cute the script after it has been downloaded.
4.	Resume pars¬ing the document.
As you can tell, this leads to a very bad user expe¬ri¬ence since the browser isint really doing any¬thing use¬ful while the script file is down¬load¬ing. To avoid this, most appli¬ca¬tions place the script tag at the bot¬tom of the html page, which is a much bet¬ter way to solve this problem.
In fact, this is exactly what the async attribute is for.
________________________________________
Async
When you add the async attribute to your script tag, the fol¬low¬ing will happen.
<script src="myfile1.js" async></script>
<script src="myfile2.js" async></script>
1.	Make par¬al¬lel requests to fetch the files.
2.	Con¬tinue pars¬ing the doc¬u¬ment as if it was never interrupted.
3.	Exe¬cute the indi¬vid¬ual scripts the moment the files are downloaded.
The great thing of this flow is that scripts can down¬load in par¬al¬lel while the doc¬u-ment is being parsed. But there’s a caveat to this and thats the third point — the script will be exe¬cuted the moment it is down¬loaded. This can be a non-issue if a script is com¬pletely self con¬tained. How¬ever, in many sit¬u¬a¬tions, scripts may depend on other scripts to have done some ini¬tial¬iza¬tion before they can exe¬cute. e.g. jquery plu¬g¬ins require the jquery vari¬able to already exist on the page.
NOTE: Scripts that you pro¬gram¬mat¬i¬cally insert into the DOM are async by default, unless you explic¬itly set their async attribute to false at inser¬tion time.
Defer
Defer is very sim¬i¬lar to async with one major dif¬fer¬er¬ence. Here’s what hap¬pens when a browser encoun¬ters a script with the defer attribute.
<script src="myfile1.js" defer></script>
<script src="myfile2.js" defer></script>
1.	Make par¬al¬lel requests to fetch the indi¬vid¬ual files.
2.	Con¬tinue pars¬ing the doc¬u¬ment as if it was never interrupted.
3.	Fin¬ish pars¬ing the doc¬u¬ment even if the script files have downloaded.
4.	Exe¬cute each script in the order they were encoun¬tered in the document.
As you can tell, defer is pretty much what you want to do in your files. How¬ever, due to lim¬ited browser sup¬port, its not a viable option at the time of writing.


30: Why is it generally a good idea to position CSS <link>s between <head></head> and JS <script>s just before </body>? Do you know any exceptions?
A: 
pted	Just to add on to what jdelStrother has mentioned about w3 specs and ARTstudio about browser rendering.
It is recommended because when you have the CSS declared before <body> starts, your styles has actually loaded already. So very quickly users see something appear on their screen (e.g. background colors). If not, users see blank screen for some time before the CSS reaches the user.
Also, if you leave the the styles somewhere in the <body>, the browser has to re-render the page (new and old when loading) when the styles declared has been parsed.


31: What is progressive rendering? answer
A: Progressive rendering is the name given to techniques used to render content for display as quickly as possible.
It used to be much more prevalent in the days before broadband internet but it's still useful in modern development as mobile data connections are becoming increasingly popular (and unreliable!)

32: Have you used different HTML templating languages before?
◦	asp.net:
◦	jsp:
◦	jsde:
◦	php: is a server-side scripting language designed for web development but also used as a general-purpose programming language.
◦	
A: asp.net, jsp and php.

CSS Questions:
33: What is the difference between classes and ID's in CSS?
A: I take a different stance than most web designers when it comes to using ID's and classes. The vast majority of CSS coders use ID's for any elements that are simply used once on a page. However, I only use classes to style my websites, but, when I want to use an element in JavaScript, I use an identifier. From a presentational standpoint, styling elements with classes looks exactly the same as styling them with ID's, but the flexibility of classes offers a certain appeal even if I don't plan on using a class more than once on a page. Also, when I see an ID in my XHTML, it reminds me that there is some JavaScript that refers to that element.


34: What's the difference between "resetting" and "normalizing" CSS? Which would you choose, and why?
A: Resetting: Removing all styling from every element - margins, padding, etc. All elements will have the same font-size, same line-height and no spacing. Eric Meyer's Reset is the most common approach: http://meyerweb.com/eric/tools/c...
Normalizing: Making elements render consistently across browsers. So all h1s will have the same size across browsers, for instance. Nicolas Gallagher's normalize.css is generally used for normalizing: http://necolas.github.io/normali...

35: Describe Floats and how they work.
A: The CSS float property is a very important property for layout. It allows you to position your web page designs exactly as you want them to display—but in order to use it you have to understand how it works.
In a style sheet, the CSS float property looks like this: .right {float: right;}
This tells the browser that everything with the class of “right” should be floated to the right.
36: Describe z-index and how stacking context is formed.
A: The z-index property in CSS controls the vertical stacking order of elements that overlap. As in, which one appears as if it is physically closer to you. z-index only effects elements that have a positionvalue other than static (the default).
CSS
Div {
   Z-index:1; /* integer */
		}

37: Describe BFC(Block Formatting Context) and how it works.
A: A Block Formatting Context is part of the visual CSS rendering of a web page in which block boxes are laid out. The positioning scheme to which it belongs is normal flow. According to W3C:
38: What are the various clearing techniques and which is appropriate for what context?
A: use clear class, inserts a hidden “.” which is used to clear the content. Simple Clearing of Floats

39: Explain CSS sprites, and how you would implement them on a page or site.
A: CSS Sprites is a method of combining multiple images used throughout your website into one big image. You can then use the proper background-position CSS attribute to load the particular image you want from your CSS Sprite using the X and Y coordinates.
When it comes to creating CSS Sprites you’ve got two options. If you’re proficient enough with a photo editing program such as Adobe Fireworks or Adobe Photoshop then you’ll have no problem creating a CSS Sprite. For people who aren’t as savvy with those sorts of programs we recommend using SpriteMe. SpriteMe is a bookmarklet. After you’ve added it to your bookmarks bar, you simply go to any website and click the SpriteMe bookmarklet. SpriteMe will then open up an overlay over the right side of your screen with everything you need. You’ll also find that there is a demo on the SpriteMe site which will greatly assist anyone who isn’t as knowledgable.


40: What are your favourite image replacement techniques and which do you use when? answer
◦	Unicode: for table
◦	font: control the size via font-size and color
◦	css3: for 3D
◦	svg: base on the image size
◦	canvas: drawing picture
	A: svg for normal image. Css3 for 3D

41: How would you approach fixing browser-specific styling issues?
A: We have taken three approaches. 
1. Using cross-browser CSS coding. 
The internet explorer is a bitch and using this on IE is very hard. 

2. Making responsive websites.
But this means having a menu button instead of a bar in many places that we don't want, it can be a problematch. 

3. Using a PHP script on the index page (without) many divs and directing based on the browser. This is in testing and takes lots of time, although results are better than the above two. 

42: How do you serve your pages for feature-constrained browsers?
◦	What techniques/processes do you use?
	A: 

43: What are the different ways to visually hide content (and make it available only for screen readers)?
A:  * Labeling a form element that has meaning conveyed visually, but not otherwise, such as inputs for search and phone number area code.
•	Providing headings where related content has meaning conveyed visually, but not otherwise, such as a menu.
•	Hiding “skip-to” links—anchor links which jump over large blocks of content on a page. These type of links should be focusable and viewable for sighted keyboard users. The most typical is a “skip to main content” link at the beginning of a web page which often jumps past the web page mast and global navigation.
•	Providing special instructions in special circumstances where interaction may be confusing to users of assistive technology. Use discretion with this, and be careful when doing so; it’s important to not be condescending like the UK Census website.


44: Have you ever used a grid system, and if so, what do you prefer?
A:  couple. Tried the classic 960 grid system in photoshop before, but now mainly uses Bootstrap's grid system

45: Have you used or implemented media queries or mobile specific layouts/CSS?
	A: One of these tricks is the use of media queries, which work to call styles to the user device based on its dimensions. There has been some debate in the past on whether media queries are the best solution when it comes to mobile first, and that debate still continues. However, the Responsive Issues Community Group (RICG) and W3C have looked at ways to implement element queries, which some believe would be a better solution. Why? Because  they don’t depend on the viewport, but on the container within it. Media queries are a simple and effective way to serve different content to a range of devices and the most commonly used queries are those that deal with the viewport’s height and width.
#wrapper (
  width: 80%;
  margin: auto;
  max-width: 1200px;
  min-width: 800px;
}
@media screen and (max-width: 800px) {
  #wrapper {
    width: 90%;
    min-width: 0;
  }
}

46: Are you familiar with styling SVG?
A: SVG, or Scalable Vector Graphics, is a XML-style markup driven vector graphic rendering engine for the browser. SVG is supported in every browser, except IE < v9 and Android < v3. The same support is available for canvas (except canvas goes all the way back on Android), so the question often surfaces: which one should you use?

47:How do you optimize your webpages for print? answer
	A: Create A Stylesheet For Print
Of course you have at least one stylesheet to control the layout of the page and formatting of the content, but do you have a stylesheet to control how your page will look like in print? Add the print style sheet, with the media attribute set to "print", at the end of the list of stylesheets in the header. This will allow you to create custom CSS classes applied only at the time of print. Make sure your structure CSS file is given a media attribute of "all."
<!-- Main stylesheet on top -->
<link rel="stylesheet" type="text/css" href="/global.css" mce_href="/global.css" href="/global.css" mce_href="/global.css" media="all" />
<!-- Print only, on bottom -->
<link rel="stylesheet" type="text/css" href="/print.css" mce_href="/print.css" hr

48:What are some of the "gotchas" for writing efficient CSS?
	A: I have a few that I’ve developed over the years. They’re quite personal, but in any case I don’t think there’s a real standard for writing CSS.
Here are a few rules I follow:
•	I write my CSS in line. I must be part of a very small minority. The thing is: I absolute love information density. I want to see the CSS structure in front of me, so I make use of the all the horizontal space. When writing 1 property per line (as everyone), it’s easy to read the properties. But I don’t care about the properties: I know them. I want to read the selectors. So I have one set of properties per line, with 1 or multiple selectors. Sometimes I put selectors on several lines, sometimes not. Depends.
•	to be able to scan my properties quickly despite the fact that they’re on single line, I put them in alphabetical order. It works pretty well with time. I know roughly where to look to find a margin or a width or a text-transform.
•	group shared properties with selectors. If several elements share a same set of properties, you could have dedicated class, or repeat yourself, or use a mixin. What I do is just list all the selectors that share this set. Then, I can have specific styles for each of these selectors. Way better than having a dedicated class.
•	I only use classes. I keep ids only for jQuery stuff. CSS priority is hard to graps, and ids are powerful selectors. They can take over the styling quite easily. To avoid headaches, I just use classes. Ids are meant to be used for unique elements. But nothing prevents from using classes like that. There’s no semantic in CSS. So use .header instead of #header, and you’ll avoid priority issues. Especially true when having #nav li, because if a li has #nav-home, you can’t use just #nav-home and it’s stupid because it’s an id selector, so the uniqueness should work. But it doesn’t because #nav li is stronger. So you have to do #nav #nav-home, which looks really stupid.
•	Here’s how I order my styles: reset, fonts, generic tags, shared properties, common elements (that appear on every page), elements, elements in context, colors (background, borders included), z-index, animations, CSS3 vendor-prefix stuff.
•	I use a tab to show a variation of the styling of an element.

49: What are the advantages/disadvantages of using CSS preprocessors? less/sass
◦	Describe what you like and dislike about the CSS preprocessors you have used.
A: Try to compare articles attached to this question. It depends what to treat as advantage or disadvantage.
Advantages:
•	global changes (e.g. colours) in one place
Disadvanteges:
•	relying on a preprocessor for any update or change (ensure consistency with preprocessor and generated CSS)
To consider:
•	nested structure
•	extensions and mixins
•	generated CSS size
Source:
•	http://www.urbaninsight.com/2012/04/12/ten-reasons-you-should-be-using-css-preprocessor
•	http://blog.millermedeiros.com/the-problem-with-css-pre-processors/
•	http://css-tricks.com/musings-on-preprocessing/
50: How would you implement a web design comp that uses non-standard fonts?
A: using @font-face
using font service link
	<link href='http://fonts.googleapis.com/css?family=Lato' rel='stylesheet' type='text/css'>
 
51: Explain how a browser determines what elements match a CSS selector.
A: Source:
•	http://programmerinnervoice.wordpress.com/2013/12/18/how-does-browser-read-css-selector/
•	http://stackoverflow.com/questions/5797014/why-do-browsers-match-css-selectors-from-right-to-left/5813672#5813672

52: Describe pseudo-elements and discuss what they are used for. answer pseudo-classes

53: Explain your understanding of the box model and how you would tell the browser in CSS to render your layout in different box models.
A: All HTML elements can be considered as boxes. The CSS box model is essentially a box that wraps around HTML elements, and it consists of: margins, borders, padding, and the actual content.
When you set the width and height properties of an element with CSS, you just set the width and height of the content area. To calculate the full size of an element, you must also add the padding, borders and margins.
IE8 and earlier versions of IE, included padding and border in the width property. To fix this problem, add a <!DOCTYPE html> to the HTML page.
 
box-sizing property:
•	content-box - (default) element width doesn’t include padding and border
•	border-box -  element width includes padding and borders
Demo: http://codepen.io/elad2412/pen/Abhdy
Source:
•	http://www.w3schools.com/css/css_boxmodel.asp
•	https://coderwall.com/p/-jeysw

54: What does * { box-sizing: border-box; } do? What are its advantages?
A: It’s the IE6 Quirks mode: if you set a width, and add paddings and borders, the totalwidth won’t change. It’s the innerwidth that’ll adapt.
Advantage? You can play with the paddings and border values without worrying about expanding your box. Very convenient for column layouts. And you can mix percentage and pixel values, so you don’t have to rely on a child element for the padding.
Disadvtange? Well, I’ve spent 7 years designing with the content-box model in mind, and now it seems he border-box model is catching up. I feel like dealing with IE6 again. But apparently, I’ve heard that the W3C always wanting to make the border-box model the standard. So I guess it’s a good idea to get acquainted with it right away. Bootstrap uses it, and my HTML5 reset uses it. And the browser compatibility seems ok.

55: List as many values for the display property that you can remember.
A: Note: The values "inline-table", "table", "table-caption", "table-cell", "table-column", "table-column-group", "table-row", and "table-row-group" are not supported in IE7 and earlier. IE8 requires a !DOCTYPE. IE9 supports the values.
Note: The values "flex" and "inline-flex" requires a prefix to work in Safari. For "flex" use "display: -webkit-flex", for "inline-flex" use "display: -webkit-inline-flex;".

56: What's the difference between inline and inline-block?
A: inline-Default value. Displays an element as an inline element(like <span>)
Inline-block: Displays an element as an inline-level block container. The inside of this block is formatted as block-level box, and the element itself is formatted as an inline-level box

57: What's the difference between a relative, fixed, absolute and statically positioned element?
A: http://www.webdevbydoing.com/whats-the-difference-between-static-relative-absolute-and-fixed-positioning/

58: The 'C' in CSS stands for Cascading. How is priority determined in assigning styles (a few examples)? How can you use this system to your advantage?
•	
59: What existing CSS frameworks have you used locally, or in production? How would you change/improve them? answer
A: Bootstrap is the most popular HTML, CSS, and JS framework for developing responsive, mobile first projects on the web

60: Have you played around with the new CSS Flexbox or Grid specs?
A: The CSS Box Model is pretty much the current mantra for organizing elements and laying out websites.  Oh the joys of floats, absolute positioning, percentage based widths, and overflow hidden. In the near (optimistic) future, Flexbox and Grid Layout are going to radically change the way we approach layout and build websites.  These new properties flip our CSS-hack approach on its head and make us consider layout from a logical perspective. Finally! In fact, the foundation of the grid layout seems to be loosely based on table based layout semantics, albeit far more flexible, adaptable, and without that gag-reflex that tends to be associated with using tables for layout.
As exciting as this is, the spec is still in its infancy and forces us to implement a plethora of vendor prefixes in order to start exploring the possibilities. All new properties need to start somewhere, so I encourage all designers to start exploring and getting your hands digitally dirty. The sooner we start applying these properties, the faster they will be implemented, but tread carefully and test, test, test.
61: How is responsive design different from adaptive design? answer
A: Google has always recommended responsive web design (RWD) and is actually due to roll out a big updateon the 21st April which will work to rank mobile-friendly sites higher.
It doesn’t specify in the update that you must use responsive design though, just that a site be accessible on mobile, with good UX and performance.
With that in mind, let’s examine the pros and cons of adaptive vs. responsive design with regards to performance and UX.
One of the biggest debates that we’ve seen since the rise of mobile is whether you should choose to develop a responsive, adaptive web design (AWD) or standalone mobile site (with its own m. URL). For the purposes of this discussion, we’ll leave out standalone m. sites as it appears to be the least favorite solution for designers and businesses since they must be created separately (which accrues more upfront cost and maintenance costs).
62: Have you ever worked with retina graphics? If so, when and what techniques did you use?
A: Pixels and Screen Density: Retina is a friendly word used by Apple to lay emphasis on the double density pixels screen of its devices. On such high resolution display screens like of Retina Ipad and MacBook Pro, it is nearly impossible for a human eye to see the pixels from a normal viewing distance.
CSS Pixel: CSS pixel is an abstract unit used by the browsers to draw images and other content on a web page. CSS pixels are DIPs which means they are device independent pixels. They readjust themselves according to the pixel density of the screen they are rendered in.
If we have the following piece of code: <div style=”width:150px; height:200px”></div> The above HTML component would look 150px by 200px in size in a standard display while 300px by 400px in a Retina display to retain the same physical size.
 


63: Is there any reason you'd want to use translate() instead of absolute positioning, or vice-versa? And why?
A: Yes, translate do not cause the browser to repaint when it is used, which if you're looking for the best performance is undoubtly better.

JS Questions:
64: Explain event delegation
A: One of the hot methodologies in the JavaScript world is event delegation, and for good reason.  Event delegation allows you to avoid adding event listeners to specific nodes;  instead, the event listener is added to one parent.  That event listener analyzes bubbled events to find a match on child elements.  The base concept is fairly simple but many people don't understand just how event delegation works.  Let me explain the how event delegation works and provide pure JavaScript example of basic event delegation.
https://davidwalsh.name/event-delegate

65: Explain how this works in JavaScript
◦	obj.foo() //get value
◦	foo() //a function
◦	foo.apply(obj) //new operator
◦	new Clazz()
A: The best way to introduce the Clazz class is by comparing it to the java.lang.Class class. Though both serve the same function as runtime meta-data about a type, there are several important differences:
•	Class is a final class embedded in the JVM. Its behavior cannot be customized or enhanced. Clazz is an abstract class and allows many alternative implementations.
•	Class describes a Java type in terms of fields, methods and constructors. Clazz describes a type in terms of properties, operations and instance factories. In the case when a Clazz represents a Java class, those properties, operations and instance factories may or may not map directly to fields, methods and constructors. The mapping is determined by the implementation of the Clazz and can be quite non-trivial. For example, a Clazz may map pairs of Java methods like getFoo() and setFoo() to a single property called "foo". There may be many ways to describe the same Java class with a Clazz.
•	Class is restricted to describing Java types. Clazz does not have that limitation. A Clazz can be created dynamically out of piece parts.
http://commons.apache.org/dormant/clazz/userguide.html

66: Explain how prototypal inheritance works
A: JavaScript has long held the dubious distinction of being both one of the world's most popular and most misunderstood programming languages. The source of the confusion is not that difficult to spot. It's really in the name. JavaScript sounds a lot like a subset of Java, when it isn't. Java is only one of the languages that JavaScript is modeled after, along with C and C++.
Moreover, despite its striking similarity to Object-Oriented (OO) languages, JavaScript itself eschews the classical inheritance models of the aforementioned languages in favor of prototypical inheritance. That can't be helping.
In this tutorial, we're going to learn more about prototypical inheritance and its ramifications in writing OO code. The eventual goal is to note how it differs from classical inheritance to determine whether or not the two can't meet somewhere in the middle.
http://www.htmlgoodies.com/html5/tutorials/javascript-prototypical-inheritance-explained.html#fbid=y4qkGMRkv_B

67: What do you think of AMD vs CommonJS?
A: 
accepted	RequireJS implements the AMD API (source).
CommonJS is a way of defining modules with the help of an exports object, that defines the module contents. Simply put a CommonJS implementation might work like this
// someModule.js
exports.doSomething = function() { return "foo"; };

//otherModule.js
var someModule = require('someModule'); // in the vein of node    
exports.doSomethingElse = function() { return someModule.doSomething() + "bar"; };
Basically CommonJS specifies that you need to have a the require() function to fetch dependencies, the exports variable to export module contents and some module identifier (that describes the location of the module in question in relation to this module) that is used to require the dependencies(source). CommonJS has various implementations, for example Node.js that you mentioned.
CommonJS was not particularly designed with browsers in mind so, it doesn't fit to the browser environment very well (I really have no source for this, it just says so everywhere, for example the RequireJS site.). Apparently this has something to do with asynchronous loading etc.
On the contrary, RequireJS implements AMD, which is designed to suit the browser environment(source). Apparently AMD started as an offspin of CommonJS Transport format and evolved into its own module definition API. Hence the similiarities between the two. The new thing in AMD is the define() -function that allows the module to declare its dependencies before being loaded. For example the definition could be:
define('module/id/string', ['module', 'dependency', 'array'], 
function(module, factory function) {
  return ModuleContents;  
});
So CommonJS and AMD are JavaScript module definition APIs that have different implementations, but both come from the same origins.
•	AMD is more suited for the browser, because it supports asynchronous loading of module dependencies.
•	RequireJS is an implementation of AMD, while at the same time trying to keep the spirit ofCommonJS (mainly in the module identifiers).
To confuse you even more, RequireJS, while being an AMD implementation, offers a CommonJS wrapper so CommonJS modules can almost directly be imported into use with RequireJS.
define(function(require, exports, module) {
  var someModule = require('someModule'); // in the vein of node    
  exports.doSomethingElse = function() { return someModule.doSomething() + "bar"; };
});

68: Explain why the following doesn't work as an IIFE: function foo(){ }();.
◦	What needs to be changed to properly make it an IIFE?
A: This is a function declaration: function foo(){ }();
There is change has to made: 
function foo(){
	// Do something
 }();
http://stackoverflow.com/questions/5403121/whats-the-difference-between-function-foo-and-foo-function

69: What's the difference between a variable that is: null, undefined or undeclared?
◦	How would you go about checking for any of these states?
A: In JavaScript, undefined means a variable has been declared but has not yet been assigned a value. null is an assignment value. It can be assigned to a variable as a representation of no value
http://stackoverflow.com/questions/5076944/what-is-the-difference-between-null-and-undefined-in-javascript

70: What is a closure, and how/why would you use one?
•	A: a closure is the local variables for a function — kept alive after the function has returned, or
•	a closure is a stack-frame which is not deallocated when the function returns (as if a 'stack-frame' were malloc'ed instead of being on the stack!).
•	function sayHello2(name) {
•	    var text = 'Hello ' + name; // Local variable
•	    var say = function() { console.log(text); }
•	    return say;
•	}
•	var say2 = sayHello2('Bob');
•	say2(); // logs "Hello Bob"
http://stackoverflow.com/questions/111102/how-do-javascript-closures-work

71: What's a typical use case for anonymous functions?
A: http://stackoverflow.com/questions/10273185/what-are-the-benefits-to-using-anonymous-functions-instead-of-named-functions-fo

72: How do you organize your code? (module pattern, classical inheritance?)
A: Classical inheritance-It's easy to understand. But, why? Because you can solve problems by comparing them with daily life. Think about it! Classes are like molds to create objects. And these objects have properties, can make actions (methods) and things can happen to them (events). It's simply that! Just like real objects! Well, not just like that but this way of thinking covers 90% of object oriented programming.
(It means that there are no classes in JavaScript.
Everything is an object and objects have prototypes which, at the same time are objects.)
Module pattern-In a short, Modular Patterns dictates how to structure our code, namely in modules that are reusable pieces and let us develop loose coupled applications. In JavaScript there are, primarily, 3 modular patterns definitions: AMD (Asyncrhonous Module Definition), CommonJS, ES Harmony
It's important to note that, in the current iteration of JavaScript (ECMA-262), it's impossible to define modules without the need of a script loader. Fortunately, the next version, JavaScript Harmony is coming and it's already available in some environments, such as No (de.js. In the meantime we can use nice script loader libraries like RequireJS and curl.js.(as lego simple but can build amazing)

Are Modular Patterns and Classical Inheritance compatible? Yes, they are! Is this architecture the best way of structuring your app? The answer is: "It depends". Depends on your app needs.

73: What's the difference between host objects and native objects? answer
A: native object:
object in an ECMAScript implementation whose semantics are fully defined by this specification rather than by the host environment.
NOTE Standard native objects are defined in this specification. Some native objects are built-in; others may be constructed during the course of execution of an ECMAScript program.

host object:
object supplied by the host environment to complete the execution environment of ECMAScript.
NOTE Any object that is not native is a host object.

74: Difference between: function Person(){}, var person = Person(), and var person = new Person()?
A: function Person(){} Declares a function (but does not execute it). It will usually have some code between the curly brackets.
var person = Person() Declares a variable (person), invokes a function (Person) and sets the value of person to the return of the function.
var person = new Person() Creates a new instance of an object based on the Person function. So the variable (person) is now an Object, not just a string or a number.

75: What's the difference between .call and .apply?
A: http://hangar.runway7.net/javascript/difference-call-apply

76: Explain Function.prototype.bind.
A: The bind() method creates a new function that, when called, has its this keyword set to the provided value, with a given sequence of arguments preceding any provided when the new function is called.
https://developer.mozilla.org/en/docs/Web/JavaScript/Reference/Global_objects/Function/bind

77: When would you use document.write()?
A: 
	Often these document.write injected scripts have dynamic strings attached to them to bust out of caching, or to send some info about the client to the ad server. I suspect your example started out as something like this
document.write("<script type='text/javascript' src='http://addomain/someadd.js?"+extrastuff+"'><\/sc" + "ript>");
but got tweaked over time, or was copied and modified by someone who didn't understand the extrastuff bit. But as you've written it there is no difference: the two ways you cite in your question are functionally the same.
http://stackoverflow.com/questions/556322/why-use-document-write

78: What's the difference between feature detection, feature inference, and using the UA string?
•	
79: Explain AJAX in as much detail as possible.
A: AJAX is a way to communicate to the server without reloading the page. Once we receive the data from the server, we can then manipulate those data and display unto certain parts of the page, this is why we don’t need to reload the page.
http://www.wandrr.io/JS-Interview-Question-Explain-AJAX-in-as-much-detail-as-possible

80: Explain how JSONP works (and how it's not really AJAX). answer
A: JSONP (JSON with Padding) is a technique used by web developers to overcome the cross-domain restrictions imposed by browsers to allow data to be retrieved from systems other than the one the page was served by.

81: Have you ever used JavaScript templating?
◦	If so, what libraries have you used?
A: How Do We Implement JavaScript Templates?
We’ll go into more detail on this with specific library examples, but essentially it’s as simple as including our chosen library, fetching our template and rendering it alongside some data. Most libraries support both inline and external templates. Inline templates are great for when we’ve got very few templates or we know that we’ll be using the included templates on each page load, but generally our templates should be external. External templates bring many benefits, chiefly that templates will never be downloaded to the client unless they are needed by the page.
mustache.js
Mustache is a multi-language, logic-less templating system. The mustache.js implementation is just one of many. So once we’re used to the (very simple) syntax, we can use it in a variety of programming languages.
Key Points
•	9kb file size (small)
•	Simple
•	No dependencies
•	No logic
•	No precompiled templates
•	Programming language agnostic
Example
<script id="template" type="x-tmpl-mustache">
  <p>Use the <strong>{{power}}</strong>, {{name}}!</p>
</script>
//Grab the inline template
var template = document.getElementById('template').innerHTML;
//Parse it (optional, only necessary if template is to be used again)
Mustache.parse(template);
//Render the data into the template
var rendered = Mustache.render(template, {name: "Luke", power: "force"});
//Overwrite the contents of #target with the rendered HTML
document.getElementById('target').innerHTML = rendered; http://www.sitepoint.com/overview-javascript-templating-engines/
82: Explain "hoisting".
A: var myvar = 'my value';   
(function() { 
  alert(myvar); // undefined 
  var myvar = 'local value'; // Variable Declarations are Hoisted
})();

83: Describe event bubbling.
A: Event bubbling and capturing are two ways of event propagation in the HTML DOM API, when an event occurs in an element inside another element, and both elements have registered a handle for that event. The event propagation mode determines in which order the elements receive the event.
<div>
    <ul>
        <li></li>
    </ul>
</div>

84: What's the difference between an "attribute" and a "property"?
A: Attributes carry additional information about an HTML element and come in name=”value” pairs. Example:<div class=”my-class”></div>. Here we have a divtag and it has a class attribute with a value ofmy-class.
Property is a representation of an attribute in the HTML DOM tree. So the attribute in the example above would have a property named className with a value of my-class.
Attributes are in your HTML text document/file, whereas properties are in HTML DOM tree. This means that attributes do not change and always carry initial (default) values. However, HTML properties can change, for example when user checks a checkbox, inputs text to textarea or uses JavaScript to change the property value.
http://jquery-howto.blogspot.ca/2011/06/html-difference-between-attribute-and.html

85: Why is extending built-in JavaScript objects not a good idea?
A: http://programmers.stackexchange.com/questions/104320/why-is-extending-the-dom-built-in-object-prototypes-a-bad-idea

86: Difference between document load event and document ready event?
A: $(document).ready() fires when the HTML has finished loading. You can’t interact with the DOM before the HTML has finished loading, so we keep all our JS interactions wrapped up in the ready handler.
Note: The ready event is just for jQuery, so that’s a downside if you weren’t planning on including all of jQuery on your site.
window.onload fires when all of the content (images, scripts, CSS, the whole lot) has finished loading. This can be really slow, so we try not to keep too much here. But it can be useful if you need to work with images of unknown size.
And that’s it! This has been the most straight forward answer yet :)

87: What is the difference between == and ===?
A: JavaScript has both strict and type-converting equality comparison. For strict equality the objects being compared must have the same type and:
•	Two strings are strictly equal when they have the same sequence of characters, same length, and same characters in corresponding positions.
•	Two numbers are strictly equal when they are numerically equal (have the same number value). NaN is not equal to anything, including NaN. Positive and negative zeros are equal to one another.
•	Two Boolean operands are strictly equal if both are true or both are false.
•	Two objects are strictly equal if they refer to the same Object.
•	Null and Undefined types are == (but not ===). [I.e. (Null==Undefined) is true but (Null===Undefined) is false]

88: Explain the same-origin policy with regards to JavaScript.
A: The “Same Origin” policy limits the access of one window to another.
The reason behind that is security. If you have blabla.com in one window and gmail.com in another one, then you’d not want a script from blabla.com to access or modify your mail or run actions in context of gmail on your behalf.
The essence of the Same Origin policy can be formulated as: windows can work in contexts of each other only if they are from same protocol://domain:port, or, shortly, from same origin.
http://javascript.info/tutorial/same-origin-security-policy

89: Make this work:
duplicate([1,2,3,4,5]); // [1,2,3,4,5,1,2,3,4,5]
A: Array.prototype.duplicate = function() { 
  var len = this.length;
  for (var i = 0; i < len; i++) {
    this[len + i] = this[i];
  }
  return this;
}
Array.prototype.duplicate = function () {
    var array = this;
    return array.concat(array);
};


90: Why is it called a Ternary expression, what does the word "Ternary" indicate?
A: http://lucybain.com/blog/2014/js-ternary/

91: What is "use strict";? what are the advantages and disadvantages to using it?
A: http://lucybain.com/blog/2014/js-use-strict/

92:Create a for loop that iterates up to 100 while outputting "fizz" at multiples of 3, "buzz" at multiples of 5 and "fizzbuzz" at multiples of 3 and 5
A: for (x=1; x <= 100; x++){
    if( x % 3 == 0 ){
        write("fizz")
    }
    if( x % 5 == 0 ){
        write("buzz")
    }
    if( x % 15 == 0 ){
        write("fizzbuzz")
    }

    if( ( x % 3 != 0 ) && ( x % 5 != 0 ) ){
        write(x)
    }
}


93: Why is it, in general, a good idea to leave the global scope of a website as-is and never touch it?
A: http://lucybain.com/blog/2014/js-dont-touch-global-scope/

94: Why would you use something like the load event? Does this event have disadvantages? Do you know any alternatives, and why would you use those?
A:

95: Explain what a single page app is and how to make one SEO-friendly.
A: https://www.getambassador.com/blog/single-page-webapp-seo

96: What is the extent of your experience with Promises and/or their polyfills?
A: http://www.joezimjs.com/javascript/polyfilling-html5-and-css3-with-modernizr/

97: What are the pros and cons of using Promises instead of callbacks?
A: promises make more than one function to be called easier.
Particular features are that 
         (a) functions can be added anywhere in the code, subject only to the promise being within scope, and
          (b) functions added after a Deferred/promise has been resolved/rejected will fire immediately.

In short promises are perfect when you deal with multiple async calls in parallel.

Check out this question. This also may help you further :
Are there any advantages to using callbacks instead of promises?

98: What are some of the advantages/disadvantages of writing JavaScript code in a language that compiles to JavaScript?
A:

99: What tools and techniques do you use debugging JavaScript code?
A: As the complexity of JavaScript applications increase, developers need powerful debugging tools to help quickly discover the cause of an issue and fix it efficiently. The Chrome DevTools include a number of useful tools to help make debugging JavaScript less painful.


100: What language constructions do you use for iterating over object properties and array items?
A: http://stackoverflow.com/questions/8312459/iterate-through-object-properties

101:Explain the difference between mutable and immutable objects.
◦	What is an example of an immutable object in JavaScript?
◦	What are the pros and cons of immutability?
◦	How can you achieve immutability in your own code?
A: Mutable objects have fields that can be changed, immutable objects have no fields that can be changed after the object is created. A very simple immutable object is a object without any field. (For example a simple Comparator Implementation).
class Mutable{
  private int value;
  public Mutable(int value) {
     this.value = value;
  }
  getter and setter for value
}
class Immutable {
  private final int value;
  public Immutable(int value) {
     this.value = value;
  }
  only getter
}

102: Explain the difference between synchronous and asynchronous functions.
A: When you execute something synchronously, you wait for it to finish before moving on to another task. When you execute something asynchronously, you can move on to another task before it finishes.
http://stackoverflow.com/questions/748175/asynchronous-vs-synchronous-execution-what-does-it-really-mean

103: What is event loop?
◦	What is the difference between call stack and task queue?
A: A job queue (sometimes batch queue), is a data structure maintained by job scheduler software containing jobs to run.
https://en.wikipedia.org/wiki/Job_queue
A call stack is a stack data structure that stores information about the active subroutines of a computer program. This kind of stack is also known as an execution stack, control stack, run-time stack, or machine stack, and is often shortened to just "the stack".
https://en.wikipedia.org/wiki/Call_stack
So in short, a job queue is a queue of things to do (usually stored persistant) and a call stack is a stack of routines.
A job would have variables assigned to it, and a call stack would be the abstract implementation. So a job could "call" a method from a call stack.
Testing Questions:
104:What are some advantages/disadvantages to testing your code?
A:

105:What tools would you use to test your code's functionality?
A:

106:What is the difference between a unit test and a functional/integration test?
A:

107:What is the purpose of a code style linting tool?
A:

Performance Questions:
108:What tools would you use to find a performance bug in your code?
A:

109:What are some ways you may improve your website's scrolling performance?
A:

110:Explain the difference between layout, painting and compositing.
A:

Network Questions:
111:Traditionally, why has it been better to serve site assets from multiple domains?
A:

112:Do your best to describe the process from the time you type in a website's URL to it finishing loading on your screen.
A:

113:What are the differences between Long-Polling, Websockets and Server-Sent Events?
A:

114:Explain the following request and response headers:
◦	Diff. between Expires, Date, Age and If-Modified-...
◦	Do Not Track
◦	Cache-Control
◦	Transfer-Encoding
◦	ETag
◦	X-Frame-Options
A:

115:What are HTTP actions? List all HTTP actions that you know, and explain them.
A:

Coding Questions:
116:Question: What is the value of foo?
var foo = 10 + '20'; 
A:1020

117:Question: How would you make this work?
add(2, 5); // 7
add(2)(5); // 7
A: 
var add = function(x,y) {
return x + y;
};

var add = function(x) {
return function(y) {
return x + y;
};};

118:Question: What value is returned from the following statement?
"i'm a lasagna hog".split("").reverse().join("");
A: "goh angasal a m'i"

119:Question: What is the value of window.foo?
( window.foo || ( window.foo = "bar" ) );
A: “bar”

120:Question: What is the outcome of the two alerts below?
var foo = "Hello";
(function() {
  var bar = " World";
  alert(foo + bar);
})();
alert(foo + bar);
A: alert1: "Hello World"
Alert2: ReferenceError:bar is not defined

121:Question: What is the value of foo.length?
var foo = [];
foo.push(1);
foo.push(2);
A:foo.length=2

122:Question: What is the value of foo.x?
var foo = {n: 1};
var bar = foo;
foo.x = foo = {n: 2};
A: foo.x === bar.x
	According to the spec, the left hand side of an assignment expression is evaluated first, even though the operator has right-to-left precedence. Thus the expression foo.x = foo = {n: 2}which is the same as foo.x = (foo = {n: 2}) is evaluated like this:
1.	Evaluate the left-hand expression foo.x to get a reference, which is where the value of the right-hand expression will be assigned to.
2.	Evaluate the right-hand expression, to to get the value that will be assigned. The right-hand side is another assignment expression, so it gets evaluated the same way:
1.	Evaluate foo to determine where to assign to.
2.	Evaluate the expression {n:2}, which creates an object, to determine the value to assign.
3.	Assign {n:2} to foo, and return {n:2}.
3.	Assign the value that the expression on the right-side evaluated to ({n:2}), to the reference that foo.x resolved to in step 1 (before foo was assigned a new value). Which is also the same as bar.x, because of the assignment bar = foo on the line before.
When this is done, the original object, that bar is still a reference to, will have an x property that references the second object created. foo is also a reference to that second object, so foo === bar.x.

123:Question: What does the following code print?
console.log('one');
setTimeout(function() {
  console.log('two');
}, 0);
console.log('three');
A:https://www.toptal.com/javascript/interview-questions

Fun Questions:
124:What's a cool project that you've recently worked on?
A: I enjoy the creative process of programming, and I enjoy that it really makes me think.

125:What are some things you like about the developer tools you use?
A: Chome Development tool- I’m not sure how I could work without Chrome Developer Tools. When I do front-end development on WordPress sites, I use it absolutely all day long, and it saves me hours every day relative to working without it.
http://wpshout.com/chrome-developer-tools-every-wordpress-developers-best-friend/

126:Do you have any pet projects? What kind?
A: yes, I will show you some in my github.

127:What's your favorite feature of Internet Explorer?
A: http://winsupersite.com/article/windows-7/internet-explorer-9-feature-focus

128:How do you like your coffee?
A: coffeescript compiles into javascript.

129: Boostrap
A: Bootstrap is the most popular HTML, CSS, and JS framework for developing responsive, mobile first projects on the web.
Bootstrap makes front-end web development faster and easier. It's made for folks of all skill levels, devices of all shapes, and projects of all sizes.
http://getbootstrap.com/

Contributors:
This document started in 2009 as a collaboration of @paul_irish @bentruyman @cowboy @ajpiano @SlexAxton @boazsender @miketaylr @vladikoff @gf3 @jon_neal @sambreed and @iansym.
It has since received contributions from over 100 developers.
