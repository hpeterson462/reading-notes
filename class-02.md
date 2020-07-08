# HTML & CSS

## Chapter 2 - *Text*

* Structural Markup - elements used to describe headings & paragraphs
1) break `<br />`
1) horizontal line `<hr />`
* Semantic Markup - provides extra info such as bold, italics, & quotations
1) bold `<strong></strong>`
1) blockquote `<blockquote cite="">`
1) strike-through `<s></s>`

## Chapter 10 - *Introducing CSS*

* invisible "boxes" around each HTML element - blockline & inline elements
* style rules associated with HTML elements `p { font-family: Arial;}`
* can chain properties to have same value `h1, h2, h3 { font-family: Arial; color: yellow}`
* link CSS to HTML document with `<link href="css/styles.css" type="text/css" rel="stylesheet">`
* cascading - last rule always applies
* Inheritance - some properties will apply to child elements to simplify code

* Selectors:
1) universal  `*`
1) child  `li>a` 
1) descendant  `p a {}`
1) adjacent sibling  `h1+p {}`
1) general sib selector  `h1~p {}`

# Javascript

## Chapter 2 - *Basic Javascript Instructions*

* script - a series of statements like a recipes
* comment to explain code (comment driven code)
* Variables - store temporary info that can change
1) declaration `let quantity;`
1) assign `let quantity = 3;`
* Data Types:
1) string
1) number
1) boolean
* Rules for naming variables:
1) must begin with letter
1) can contain letters, symbols, numbers, or underscore
1) can't use keywords
1) case sensitive
1) use name that describes the info stored
1) use camelCase
* Arrays - special type of variable that stores a list of values
* values are accessed & changed from an array by index number `[0, 1, 2]`
* expressions equal a single value `let area = 2 * 3;` `const = 'beige'` and rely on operators `+ * - / < > ++ -- % && ||`

