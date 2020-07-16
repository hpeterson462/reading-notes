# Javascript

## Chapter 3 - *Object Literals*

* Object Model - series of variables and functions that represent real world scenario

* 3 Types: 
    * Browser object model
        * window, document, history, location, nav, screen
        * eg: `<window.innerHeight>`
    * Document object model
        * document, html, head, body, div, p
        * eg: `<document.title>'`
    * Global 
    Javascript Objects
        * string, number, Boolean, date, math, Regex
        * eg: `<toUpperCase>`
* 6 Data Types -
    * Primative: 
    1) String
    1) Number
    1) Boolean
    1) Undefined
    1) Null
    * Object
* Number Object - 
    * `isNan()`
* Math Object - 
    * `Math.PI`
* Date Object - 
    * `let today = new Date();`
    * `getDate()`


## Chapter 5 - *Document Object Model*

* DOM represents the page in the browser
* DOM trees have 4 nodes: 
    1) Document
    1) Element
    1) Attribute
    1) Text
* Select elements by id or class
    `getElementById()`
    * `getElementByClassName`
* DOM query will return NodeList if it can return more than one element
    * `getElemntsByTagName`
* Select element from NodeList
    * specify index number with `item()`
* Parent - sibling - firstChild
* can add/remove text content of HTML
    * `elemnet.innerHTML` - can place malicious code in site
    * `removeEl.parentNode`
* can use Chrome & Firefox to examine DOM


## Article - *Understand Domain*

* Understand the problem domain
    * take a part of the problem and narrow focus
    * talk & understand problem before coding
