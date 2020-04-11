### Postman
You can perform a volumes search by sending an HTTP GET request to the following URI:https://www.googleapis.com/books/v1/volumes?q=search+terms
This request has a single required parameter:

**q**- Search for volumes that contain this text string. There are special keywords you can specify in the search terms to search in particular fields, such as:
- intitle: Returns results where the text following this keyword is found in the title.
- inauthor: Returns results where the text following this keyword is found in the author.
- inpublisher: Returns results where the text following this keyword is found in the publisher.
- subject: Returns results where the text following this keyword is listed in the category list of the volume.
- isbn: Returns results where the text following this keyword is the ISBN number.
- lccn: Returns results where the text following this keyword is the Library of Congress Control Number.
- oclc: Returns results where the text following this keyword is the Online Computer Library Center number.

#### If the request succeeds, the server responds with a 200 OK HTTP status code 
For applications that need quick templating, there are many options that we can use like:
## EJS(Easy javascript)
 EJS is a simple templating language that lets you generate HTML markup with plain JavaScript

## Tags
 <% 'Scriptlet' tag, for control-flow, no output
<%_ ‘Whitespace Slurping’ Scriptlet tag, strips all whitespace before it
<%= Outputs the value into the template (HTML escaped)
<%- Outputs the unescaped value into the template
<%# Comment tag, no execution, no output
<%% Outputs a literal '<%'
%> Plain ending tag
-%> Trim-mode ('newline slurp') tag, trims following newline
_%> ‘Whitespace Slurping’ ending tag, removes all whitespace after it

## Includes
Includes are relative to the template with the include call. (This requires the 'filename' option.) 
## Caching
EJS ships with a basic in-process cache for caching the intermediate JavaScript functions used to render templates. It's easy to plug in LRU caching using Node's `lru-cache` library
If you want to clear the EJS cache, call ejs.clearCache

## Layouts
EJS does not specifically support blocks, but layouts can be implemented by including headers and footers

We also have to set EJS as the view engine for our Express application using app.set **('view engine', 'ejs');**.

