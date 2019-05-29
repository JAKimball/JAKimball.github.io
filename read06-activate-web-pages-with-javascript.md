# Read 06: Activate web pages with JavaScript

- HTML: the content layer
  - .html files
- CSS: the Presentation layer
  - .css files
- javascript: The Behavior Layer
  - .js files

These layers form the basis of the progression enhancement approach to web page building.

1. HTML only
2. HTML + CSS
3. HTML + CSS + JAVASCRIPT

The `<script>` element is used to load the JavaScript file into the page.

```html
<script src="js/add-content.js"></script>
```

## Placing the script in the page

```html
<script>document.write('<h3>Welcome!</h3>');</script>
```

## Javascript runs where it is found in the HTML

Moving the script will affect where the `document.write();` method will write on the page.

# Basic JavaScript Instuctions

## Statements

Individual instructions or steps are known as statements.

Statements can be organized into code blocks.

Javascript is case sensitive.

## Comments

- multiline comments begin with `/*` and end with `*/`
- single line comments begin with `//` and the javascript interpreter will ignore the rest of the line.

## Variables

Variables store temporary information for the script to operate.

Variables are declared with the `var` keyword.

```js
var quantity;
```

Variables are assigned with an assignment operator.

```js
quantity = 6;
```

## Data Types

- Numberic
- String
- Boolean

Javascript also has:

- arrays
- objects
- undefined
- null

## Rules for naming variables

1. The name must begin with a letter, dollar sign ($), or an underscore (_).  It must not start with a number.
2. It can contain letters, numbers, $, or _.  It must not include a dash (-) or a period (.).
3. It can not be a keyword or reserved word.
4. All variables are case sensitive.
5. Use a name the describes to information the variable stores.
6. If your name is made up of more than one word, use the camel case convention - a capital letter for the first letter of eavery word *after* the first.



[Return Home](/)