# HTML & CSS

## Chapter 15 - *Layout*

* `<div>` containing elements
* Block Level Elements:
    * `<h1>` `<p>` `<ul>` `<li>`
* Inline Elements:
    * `<img>` `<b>` `<i>`
* Positioning Schemes:
    * Normal - block level element appears static on a new line
    * Relative - shifts element to top, right, bottom, or left from normal
    * Absolute - positions element in relation to containing element - moves as user scroll up and down page
    * Fixed - fixes element in browser window - doesn't move as user scrolls up and down
    * Floating - shifts element right or left in block level
* Z-Index - overlapping properties (1 top, 10 bottom)
* Fixed Layout:
    * Pros - 
        * controls pixel values, position, and size of images
        * control text line length
    * Cons - 
        * gaps around edge of page
        * page can look smaller if user screen is bigger than designer screen
        * doesn't fit all screen sizes
        * page will often take up more vertical space
* Liquid Layout:
    * Pros - 
        * pages expand and contract to fit screen size
    * Cons - 
        * unexpected design control
        * text can stretch for long lines or narrow
        * image can overflow container
* keep pages within 960-1000 pixels wide
* can include multiple CSS files in one page



# Javascript

## Chapter 10 - *Error Handling & Debugging*

* Order of Execution - how scripts are processed
* Execution Contexts:
    * global context, function context, eval context 
    * variable scope - global, local
* JS interpreter processes one line of code at a time
    * When statement needs data from another function, it stacks (piles) the new function on top of the current task
* Execution Context and Hoisting
    * Execution Context has 2 Phases:
        1) Prepare
            1) new scope created
            1) variables, functions, arguments created
            1) value of `this` keyword is determined
        1) Execute
            1) assign values to variables
            1) reference functions and run code
            1) execute statements
* JS has Lexical Scope:
    * Functions are linked to the object they were defined in
    * Children can access info from Parents, but Parent cannot access from Children
* Error Objects:
    * Properties:
        * name - type of execution
        * message - description
        * fileNumber - name of JS file
        * lineNumber
    * Object:
        * Error - generic 
        * SyntaxError - syntax not followed
        * ReferenceError - variable not declared or within scopes
        * TypeError - unexpected data type
        * URIError - encodeURI(), decodeURI() used incorrectly
        * EvalError - eval() function used incorrectly
* Deduction - where is the problem? what is the problem?
* Dev Tools
* Breakpoints
* Try, Catch, Finally
    * Try - execute this code
    * Catch - if there is an exception, run this code
    * Finally - always gets executed
* Throwing Error - `throw new Error(message);`
* some problems are browser specific
* remove parts of code to see what's working
* explain code - comment code, rubber ducking
* data type issues
* spelling errors