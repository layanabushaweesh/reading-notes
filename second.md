# jQuery 
* offers a simple way to achieve a variety of common 
JavaScript tasks quickly and consistently, across all major 
browsers and without any fallback code needed.


 ## WHY USE JQUERY? 
* jQuery doesn't do anything you cannot achieve with pure JavaScript. 
It is just a JavaScript file but estimates show it has been used on over a 
quarter of the sites on the web, because it makes coding simpler. 

## FINDING ELEMENTS 
* Using jQuery, you usually select elements 
using CSS-style selectors. It also offers some 
extra selectors

>LOOPING 
In plain JavaScript, if you wanted 
to do the same thing to several 
elements, you would need to 
write code to loop through all of 
the elements you selected. 
c07/ js/ looping .js 
With jQuery, when a selector 
returns multiple elements, you 
can update all of them using the 
one method. There is no need to 
use a loop. 
$('l i em') .addClass('seasonal ') ; 
$( ' li .hot') .addClass('favorite'); 

 ## GETTING AT CONTENT 
* On this page you can see variations on how the . html() and . text() 
methods are used on the same list (depending on whether <ul >or <l i > 
elements are used in the selector). 


> .before() 
This method inserts content 
before the selected element(s) . 
.prepend() 
This method inserts content 
inside the selected element(s), 
after the opening tag. 
.after() 
This method inserts content 
after the selected element(s). 
.append() 
This method inserts content 
inside the selected element(s), 
before the closing tag. 

> attr() 
This method can get or set a 
specified attribute and its value. 
To get the value of an attribute, 
you specify the name of the 
attribute in the parentheses. 
$( ' li#one').attr('id'); 
To update the value of an 
attribute, you specify both the 
attribute name and its new value. 
$('li#one').attr('id' , 'hot ' ); 
. addCl ass() 
This method adds a new value 
to the existing value of the cl ass 
attribute. It does not overwrite 
existing values. 
. removeAttr() 
This method removes a specified 
attribute (and its value). You just 
specify the name of the attribute 
that you want to remove from the 
element in the parentheses. 
$('1 i #one') . removeAttr (' i d' }; 
.removeClass() 
This method removes a value 
from the cl ass attribute, leaving 
any other class names within 
that attribute intact

* CHANGING CSS RULES 
This example demonstrates how 
the • css () method can be used 
to select and update the CSS 
properties of elements. 
JAVASCRIPT 
$(function() { 
The script checks what the 
background color of the first list 
item is when the page loads and 
then writes it after the list. 
G) var backgroundCo l or = $ ( 'l i ' ). css ('background-col or'); 
Next, it updates several CSS 
properties in all list items using 
the same . css () method with 
object literal notation. 

 * ADDITIONAL PARAMETERS 
FOR EVENT HANDLERS 
The • on () method has two optional properties that let you: 
Filter the initial jQuery selection to respond to a subset of the elements; 
Pass extra information into the event handler using object literal notation. 

 * Reasons for Pair Programming
1. Greater efficiency
2. Engaged collaboration
3. Learning from fellow students
4. Social skills
5. Job interview readiness

