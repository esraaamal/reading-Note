# Javascript Templating
**Javascript templating** is a fast and efficient technique to render client-side view templates with Javascript by using a JSON data source. The template is HTML markup, with added templating tags that will either insert variables or run programming logic.
The template engine then replaces variables and instances declared in a template file with actual values at runtime, and convert the template into an HTML file sent to the client.

### Mustache:

Mustache is a logic-less template syntax. It can be used for HTML, config files, source code — anything. It works by expanding tags in a template using values provided in a hash or object.
It is often referred to as “logic-less” because there are no if statements, else clauses, or for loops. Instead, there are only tags. Some tags are replaced with a value, some nothing, and others a series of values.
mustache.js is an implementation of the mustache template system in JavaScript. It is often considered the base for JavaScript templating. And, since mustache supports various languages, we don’t need a separate templating system on the server side.
### This is Mustache syntax to show that it is a placeholder.
Mustache.render(“Hello, {{name}}”, { name: “Sherlynn” });
// returns: **Hello, Sherlynn**

## FlexBox
#### justify-content:
•	flex-start: Items align to the left side of the container.
•	flex-end: Items align to the right side of the container.
•	center: Items align at the center of the container.
•	space-between: Items display with equal spacing between them.
•	space-around: Items display with equal spacing around them.

#### aligns-items:
***This CSS property aligns items vertically and accepts the following values:***
•	flex-start: Items align to the top of the container.
•	flex-end: Items align to the bottom of the container.
•	center: Items align at the vertical center of the container.
•	baseline: Items display at the baseline of the container.
•	stretch: Items are stretched to fit the container.

#### flex-direction.
***This CSS property defines the direction items are placed in the container, and accepts the following values:***
•	row: Items are placed the same as the text direction.
•	row-reverse: Items are placed opposite to the text direction.
•	column: Items are placed top to bottom.
•	column-reverse: Items are placed bottom to top.

#### flex-wrap property
 ***which accepts the following values:***
•	nowrap: Every item is fit to a single line.
•	wrap: Items wrap around to additional lines.
•	wrap-reverse: Items wrap around to additional lines in reverse.

#### flex-flow
The two properties flex-direction and flex-wrap are used so often together that the shorthand property flex-flow was created to combine them. This shorthand property accepts the value of one of the two properties separated by a space.
For example, you can use flex-flow: row wrap to set rows and wrap them.


