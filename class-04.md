# HTML & CSS

## Chapter 4 - *Links*

* `<a href=""></a>`
* Absolute link - links to outside website with full address `<a href="http://www.kittenpage.com"></a>`
* Relative link - links to other pages in same site with shorthand address `<a href="index.html></a>"`
* Directory Structure:
    * Root (parent)
    * Folder (child)
* Email link - `<a href="mailto:jon@example.com"></a>`
* Link in Page - use #id to link 
    * `<a href="#top"></a>` will link to `<h1 id="top"></h>` at top of page
* Link to Another Page - url and #id 
    * `<a href="http:/www.kittenpage.com/#bottom></a>`

## Chapter 15 - *Layout*

* `<di></div>` sections that need to be boxed together
* Block-Level Elements - `<h1> <p> <ul> <li>`
* Inline Elements - `<img> <b> <i>`
* Positioning Schemes: 
    * Normal Flow - every block-level element appears new line (will not appear next to each other) `position: static`
    * Relative Positioning - moves elements from the normal position it would be to top, right, bottom, or left (doesn't affect position of surrounding elements) `position: relative`
    * Absolute Positioning - positions element in relation to its parent element (moves as page scrolls) `position: absolute`
    * Fixed Positioning - positions elements in relation to browser window (don't move when scrolled) `position: fixed`
    * Floating Elements - position element to far right or left of parent box (becomes block-level around which other content will flow) `position: float`
    * Z-Index - controls which box appears on top `z-index: 1`
* Screen Sizes:
    * iPhone - 960 x 640
    * iPad - 1024 x 768
    * MacBook - 1280 x 800
    * iMac - 2560 x 1440
* keep pages within 960-1000px wide - main info of site within top 600px.
* Fixed Width Layout - doesn't change size with browser window
* Liquid Layouts - stretch and contract with browser size change (usually use % eg. 3 columns = 33%)
* CSS style sheets can be modular to create separate sheets to control typography, layout, forms, tables, etc. 
* CSS frameworks create rules for common tasks
 
 # Javascript

## Chapter 3 - *Functions, Methods, & Objects* 

* Functions: 
    * tools to help perform a task
    * store a step to execute when called
    * name describes what function is doing
    * Parameters - info passed to function
    * Declared Function (first): 
        1) `function sayHello(){document.write('Hello');}`
        1) `function getArea(width, height){
            return width * height;
        }`
    * Call: 
        1) `sayHello();`
        1) `getArea();`
    * Function Expression 
        *can't be read before interpreter gets to it - code above can alter what goes into function   
        1) `const area = function(width, height) { return width * height;
        }`
    * Anonymous Function: no name
    * Immediately Invoked Expressions (IFFE): 
        * variable will hold value of function instead of being stored to be called later
        1) `const area = (function() {
            let width = 3; let height = 2; return width * height;
        }());`
    * Anonymous & IFFE used when code is only needed to run once
* Variable Scope:
    * Local - function-level
        * `function getArea(width, height){
            let area = width * height;
            return area;
        }`
    * Global - used anywhere in script (use more memory)
        * `const wallSize = getArea(3, 2); document.write(wallSize);`