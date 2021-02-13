# JavaScript
> WHAT IS AN OBJECT?
* Objects group together a set of variables and functions to create a model
of a something you would recognize from the real world. In an object,
variables and functions take on new names. 
>IN AN OBJECT: VARIABLES BECOME
KNOWN AS PROPERTIES 
>IN AN OBJECT: FUNCTIONS BECOME
KNOWN AS METHODS
> Creating new objects
JavaScript has a number of predefined objects. In addition, you can create your own objects. You can create an object using an object initializer. Alternatively, you can first create a constructor function and then instantiate an object invoking that function in conjunction with the new operator.
> you can also access properties using square brackets.
* for an example                   var hote l = {
                                                  name: 'Quay',
                                                  rooms: 40,
                                                   booked : 25,
                                                checkAvailability: function() {
                                               return this.rooms - this.booked;
                                                      }

## The Document Object Model (DOM) 
> The Document Object Model (DOM) specifies
how browsers should create a model of an HTML
page and how JavaScript can access and update the
contents of a web page while it is in the browser window. 

* The browser represents the page using a DOM tree.
* DOM trees have four types of nodes: document nodes,
element nodes, attribute nodes, and text nodes.
* You can select element nodes by their id or class
attributes, by tag name, or using CSS selector syntax.
* DOM query can return more than one
node, it will always return a Nadel i st.
* an element node, you can access and update its
content using properties such as textContent and
i nnerHTML or using DOM manipulation techniques.
* An element node can contain multiple text nodes and
child elements that are siblings of each other.
* In older browsers, implementation of the DOM is
inconsistent (and is a popular reason for using jQuery).
Browsers offer tools for viewing the DOM tree . 
