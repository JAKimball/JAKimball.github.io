# Read 05: Design web pages with CSS

## Thinking Inside the Box

To understand how CSS works, image an invisible box around every HTML element.

## Block and Incline Elements

- Block level elements look like they start a new line
  - `<h1>` - `<h6>`
  - `<p>`
  - `<div>`
- Inline elements flow within the text and do not start on a new line
  - `<b>`
  - `<i>`
  - `<img>`
  - `<em>`
  - `<span>`

CSS allows you to create rules for the presentation of each individual box and its contents.

CSS style rules are made up of selectors and declarations.

Selectors indicate the HTML elements the rules apply to.

Declarations indicate how the elements the selector refers to should be styled.

Declarations are each made up of two parts, a property and a value.

Several properties can be included in a declaration separated by semicolons.

Properties indicate aspects of the element to be changed such as color, font, width, height, border.

Values specify the settings for those properties.

## Link to External CSS

A link to an external CSS file will take the following form within the `<head>` element.

```html
<head>
    <link href="css/styles.css" type="text/css" rel="stylesheet" />
</head>
```

## Using Internal CSS

CSS rules can also be placed within a `<style>` element, usually in the `<head>` element of the page.

<table>
	<tr>
		<td><h3> Selector </h3></td>
		<td><h3> Meaning </h4></td>
		<td><h3> Example </h4></td>
	</tr>
	<tr>
		<td><h4> Universl Selector </h4></td>
		<td>Applies to all elements in the document</td>
		<td><code> * {} </code></td>
	</tr>
	<tr>
		<td><h4> Type Selector </h4></td>
		<td>Mathes element names</td>
		<td><code> h1, h2, h3 {} </code></td>
	</tr>
	<tr>
		<td><h4> Class Selector </h4></td>
		<td>Matches elements with matching class attributes</td>
		<td><p><code> .note {} </code></p><p><code> p.note {}</p></td>
	</tr>
	<tr>
		<td><h4> ID Selector </h4></td>
		<td>Matches by id attribute</td>
		<td><code> #intro {} </code></td>
	</tr>
	<tr>
		<td><h4> Child Selector </h4></td>
		<td> Matches element that is a direct child of another</td>
		<td><code> li>a {} </code></td>
	</tr>
	<tr>
		<td><h4> Decendant Selector </h4></td>
		<td>Matches element that is a direct child of another</td>
		<td><code> p a {} </code></td>
	</tr>
	<tr>
		<td><h4> Adjacent Sibling Selector </h4></td>
		<td>Matches element that is the next sibling of another</td>
		<td><code> h1+p {} </code></td>
	</tr>
	<tr>
		<td><h4> General Sibling Selector </h4></td>
		<td>Matches element that is a sibling of another but it does not have to be the directly preceding element</td>
		<td><code> h1~p {} </code></td>
	</tr>
</table>

## How CSS Rules Cascade

Understanding how CSS rules cascade will allow you to write simpler style sheets by creating general rules for must elements and then override them for properties of specific elements that need to appear differently.

Generally the more specific selector will determine the which will take precedence when more than one rule applies to a property of an element.  If two selector have identical specificity, the latter of the two will take precedence.

## Inheritance

The values of some properties are inherited from parent elements to child elements.  You can force properties that would not ordinarily be propagated to child elements by using the `inherit` value of the properties.

## Testing for Browser Quirks

Online tools to test site in multiple browsers:
- browsercam.com
- Browserlab.adobe.com
- Browsershots.org
- Crossbrowsertestgin.com

Browser Bug sites:
- Positioniseverything.net
- Quirksmode.org

Include MDN is your Google Search for all things MDN!

https://color.adobe.com/create

## Color

- Foreground color is the color of text.
- Background color is the color of the remaining space inside an element out side of the text.

Color can be specified in a number of ways
- RGB values - `rgb(123,22,34)`
- Hex codes - `#6af703`
- Color names - Red

CSS3 allows an opacity value
- RGBA - `rgba(123,22,34,0.5)`

CSS3 also introduces HSL colors.  The components of HSL are:
- Hue - 0 to 360
- Saturation - 0% to 100%
- Lightness - 0% to 100%

`hsl(360,100%,50%)`

Alpha is the added value for opacity.  This is a number from 0 to 1.0.

`hsla(360,100%,50%,0.5)`

[Return Home](/)