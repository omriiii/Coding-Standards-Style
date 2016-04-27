# my personal coding standards and style
Hi! This is my personal coding standards and style when I make my own wbesites. I made this repository for the sake of documentation, **to get myself to think about my code**, and to hopefully give other developers some ideas.


I ~~stole~~ got the idea from [thelifemgmt](https://github.com/thelifemgmt)'s [Coding Standards & Styleguide](https://github.com/thelifemgmt/coding_standards "thelifemgmt's Coding Standards & Styleguide")

**Some good reference links**

* http://csswizardry.com/2013/01/mindbemding-getting-your-head-round-bem-syntax/
* Another Link
* Another Link

https://css-tricks.com/centering-css-complete-guide/

https://gsnedders.html5.org/outliner/
## HTML Formatting Rules
*** NOT FINISHED !! ***

* Always indet child every child element.
* Always indet using *only* the "tab" character `(ascii: 9)`. Never use "space" characters `(ascii: 32)`. 
* Always include an `alt=""` attribute to `<img>` tags.
* Avoid using `"` and `'` in your content. Use `&lsquo;`/`&rsquo;`, `&ldquo;`/`&rdquo;` (`‘`, `’`, `“`, `”`) instead. 
* Never close self-closing tags such as `<hr>`, `<br>`, `<img>`, or `<input>`.
* Never use inline css or inline javascript

Example:
```
<main>
	<img src="url(/res/imgs/latte_coffee.png)" alt="A picture of a good old cup of coffee.">
	<!-- Some more code coming soon -->
</main>
```

## Head tag & Type Attributes

* Always comment segemnts in the `<head>` tag. Eg. "Libraries", "Stylesheets", "Meta tags", etc.
* Never add a`type="text/css"` attribute to stylesheet `<link>` tags.
* Never add a `type="text/javascript"` attribute to javascript `<script>` tags.

In HTML5 the default value for the `type` attribute will always be text so it's not needed with those two tags.

Example:
```
<head>
    <!-- PAGE INFO & META TAGS -->
	<!---------------------------------------------->
	
	<meta charset="UTF-8">
	<meta name="author" content="Omrii">
	<meta name="description" content="Head tag & Type Attributes example.">
	<title>Title of page</title>
		
		
	<!-- LIBRARIES -->
	<!---------------------------------------------->

	<!-- BOOTSTRAP CSS -->
    <link href="/res/libs/css/bootstrap.min.css" rel="stylesheet">
    
	<!-- JQUERY JS -->
    <script src="/res/libs/js/jquery.min.js"></script>`
    
</head>
```

## CSS3 Animations
*** NOT FINISHED !! ***

* Always use the `transform` property when animating elements with CSS.
* You have a lot of options! Pick the best ones: https://api.jqueryui.com/easings/

## Project Organization
*** NOT FINISHED !! ***

* Always keep two directories for your project, `src` (for Source) and `dist` (for Distribution)
* `src` will include all of the files of the project before compilation and concatnation. 
* `dist` will include only concatnated and compiled assets. Do not include SASS files.

Things to think about:
* Different html pages that are included in the website. includes directory maybe? (things like navbar.html)

Example:
```
//root
|
├── views //All of the pages in the website.
|   ├── page0.php //Eg. Homepage
|   ├── page1.php //Eg. About Us
|   └── page2.php //Eg. Contact Us
|
├── libs //(Libraries)
|   ├── css
|   |   ├── bootstrap.css
|   |   └── bootstrap.min.css
|   |
|   └── js
|       ├── jQuery.js
|       ├── jQuery.min.js
|       ├── angularJS.js
|       └── angularJS.min.js
|
└── res //(Resources)
    ├── css
    |   └── style.css //compiled and concatnated style.scss
    |
    ├── graphics
    |   ├──   picture0.png
    |   ├──   picture0.jpg
    |   ├──   logo.svg
    |   └──   favicon.ico
    |
    ├── js
    |   ├──   app.js
    |   └──   functions.js
    |
    ├── sass
    |   └── style.scss
    |       └── project
    |           ├── _project-fonts.scss
    |           ├── _project-styles.scss
    |           ├── _project-variables.scss
    |           |
    |           ├── components
    |           |   ├── _buttons.scss
    |           |   ├── _lists.scss
    |           |   └── _inputs.scss
    |           |
    |           ├── partials
    |           |   ├── _header.scss
    |           |   ├── _masthead.scss
    |           |   └── _footer.scss
    |           |   
    |           └── globals
    |               ├── _mixins.scss
    |               ├── _typography.scss
    |               ├── _reset.scss
    |               └── _base.scss
    |
    └── fonts
        ├──   font0.ttf
        ├──   font0.eot //.eot is used for IE
        ├──   font1.ttf
        └──   font1.eot //.eot is used for IE
```


## Website testing
Sometimes you will overlook/misuse your markups. Use these websites to check if they're okay.
* https://gsnedders.html5.org/outliner/ (Example article: https://www.smashingmagazine.com/2011/08/html5-and-the-document-outlining-algorithm/)
* http://html5doctor.com/
- 

### Notes
Some more stuff coming `soon™`.

I left this GitHub editor style link here for me becasue I know I'll need it again at some point.
[don't mine me c:](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet "(old man voice) GET OUTTA HERE!!")
