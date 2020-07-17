# HTML & CSS

## Chapter 7 - *Forms*

* Captures user information:
    * text
    * choices - radio buttons, checkboxes, dropdown menus
    * submitting form
* How forms work: 
    1) user fills in for
    1) form control sent to server
    1) server processes info using PHP, C#, VB.net, or Java (may store in database)
    1) server creates new page and sends back
* Info sent to browser uses name-value pairs `name=value`
* Form Structure: `<form action=""><label type=""><input type="">`
* Every form requires action attribute: `<form action="">`
* Can also have method attribute: `<form action="" method="">`
* Input Type - 
    * Text: `<input type="text" name="" size="" maxlength="">` 
    * Password: `<input type="password" name="" size="" maxlength="">` 
    * Text Area: `<input type="textarea" name="" cols="" rows="">`
    * Radio Button: `<input type="radio" name="" value="" checked="">`
    * Checkbox: `<input type="checkbox" name="" value="" checked="">`
    * Dropdown: `<select name=""><option value="">`
    * Multiple Select Box: `<select name="" size="" multiple=""><option value="" selected="">`
    * Date `<input type="date" name="">`
    * File `<input type="file" name="">`
    * Submit Button `<input type="submit" name="" value="">`
    * Image Button `<input type="image" src="" width="" height="">`
    * Email `<input type="email" name="">`
    * Search `<input type="search" name="">`
    * Button & Hidden Controls - can combine text and images surrounded by button; use hidden to store info without being seen by user `<input type="hidden" name="" value="">`
    * Title group inputs `<legend></legend>`
    * Group inputs together `<fieldset></fieldset>`
* Form Validation - message if form hasn't been filled out correctly (only Chrome & Opera support right now)


## Chapter 14 - *Lists, Tables, & Forms*

* CSS can control list, tables, and forms by using list-style-type and list-style-image properties
* Use CSS to control table cells that can have different appearances in different browsers
* Style submit buttons, text inputs, and legends
* Align form controls vertically for ease of user experience
    * Use float, width, and align-text
* Cursor styles - auto, crosshair, default, pointer, move, text, wait, help, url("cursor.gif")
* Web Dev tool for HTML/CSS


# Javascript

## Chapter 5 - *Events*

* Events indicate what to do when something happens - triggers JS function
* Binding - states which event you are waiting for and which element will respond
* Use event delegation to monitor events that happen to child elements
* Event Types: 
    * UI
    * Keyboard
    * Mouse
    * Focus
    * Form
    * Mutation
* How events trigger JS code:
    1) select element
    1) specify event
    1) run code
* 3 ways to bind element to event:
    * HTML event handlers
    * traditional DOM event handlers
    * DOM level 2 even listeners
* Don't use HTML event handlers
* DOM Event Handler: `element.onevent = functionName`
* Event Listener: `element.addEventListener('event', functionName, [Boolean])`
* Parameters can be used in handlers and listeners
* Event bubbling vs event capturing
* Flow matters - containing child elements use less memory and delegates jobs
* Event Object - tells info about event and element it happened on
* Change default behavior: 
    * `preventDefault()` 
    * `stopPropagation`
* Types of events: 
    * DOM
    * HTML
    * BOM (browser object model) - UI events
