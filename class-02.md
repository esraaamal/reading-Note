# jQuery it makes coding simpler. 

**JQuery is a javascript file that we include  in our web pages it lets us find** **element using Css-style
 selector and then do something with the element using** **jQuery methods, its also*****offers a simple way to achieve a variety of common***
***JavaScript tasks quickly and consistently, across all major***
***browsers and without any fallback code needed.***


**Most people who use jQuery do not try to understand how the jQuery JavaScript file achieves**
what it does. As long as you
know how to select elements
and how to use its methods and
properties, you can reap the
benefits of using jQuery without
looking under the hood.

1: SIMPLE SELECTORS
it is not always easy to select the elements
that you want to. For example:
• **Older browsers** do not support the latest
methods for selecting elements.
• **IE** does not treat whitespace between elements
as text nodes, while other browsers do.
Such issues **make it hard** to select the right elements
on a page across all major browsers.
Rather than learn a new way to select elements,

**jQuery** uses a language that is already familiar to
front-end web developers: CSS selectors. They:
• Are much faster at selecting elements
• Can be a lot more accurate about which elements
to select
• Often require a lot less code than older DOM
methods
• Are already used by most front-end developers 

2: COMMON TASKS IN LESS CODE
There are some tasks that front-end developers
need to do regularly, such as loop through the
elements that have been selected.
**jQuery**has methods that offer web developers
simpler ways to perform common tasks, such as:
• loop through elements
• Add I remove elements from the DOM tree
• Handle events
• Fade elements into I out of view
• Handle Ajax requests 

**jQuery's** motto is "Write less, do more," because it allows you to achieve
the same goals but in fewer lines of code than you would need to write
with plain JavaScript. 
### WORKING WITH EACH ELEMENT IN A SELECTION 
 **each()**
Allows you to perform one or
more statements on each of
the items in the selection of
elements that is returned by a
selector - rather like a loop in
JavaScript.
It takes one parameter:
a function containing the
statements you want to run on
each element. 

**this** or **$(this)**
As the . each() method goes
through the elements in a
selection, you can access the
current element using the this
keyword.
You also often see $ (thi s),
which uses the this keyword to
create a new jQuery selection
containing the current element.
It allows you to use jQuery

#### EVENTS :
**Every event handling function receives an event object**.
It has methods and properties related to the event that occurred. 

The • **on** () method has two optional properties that let you:
Filter the initial jQuery selection to respond to a subset of the elements;
Pass extra information into the event handler using object literal notation. 


#### How to inclide JQuery in our page:
LOADING JQUERY FROM A CDN 