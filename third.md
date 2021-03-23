## Mustache
* Javascript templating is a fast and efficient technique to render client-side view templates with Javascript by using a JSON data source. The template is HTML markup, with added templating tags that will either insert variables or run programming logic.

* Mustache is a logic-less template syntax. It can be used for HTML, config files, source code — anything. It works by expanding tags in a template using values provided in a hash or object.

* Mustache.render(“Hello, {{name}}”, { name: “Sherlynn” });
// returns: Hello, Sherlynn
Whereby the first parameter ‘hello’ refers to the hello.html file (no need to include the extension (e.g. hello.html) as it has been previously set as HTML.

* The second parameter would be the JSON data itself. We can also pass in a variable representing the data, for example:

* var nameObject = {"name": "Sherlynn"}
res.render('hello', nameObject)

## A Guide to Flexbox
Background:
> The main idea behind the flex layout is to give the container the ability to alter its items’ width/height (and order) to best fill the available space (mostly to accommodate to all kind of display devices and screen sizes). A flex container expands items to fill available free space or shrinks them to prevent overflow.

.container {
  display: flex; /* or inline-flex */
  /* this enables flex content for all its direct children */

  flex-direction: row | row-reverse | column | column-reverse;
  /* default | from right to left | top to bottom | bottom to top */

  flex-wrap: nowrap | wrap | wrap-reverse;
  /* default, all elements on one line | flex items will wrap onto multiple lines | like previous but from bottom to top */

  flex-flow: row nowrap | column wrap | etc etc;
  /* this is a shorthand for flex-direction and flex-wrap */

  justify-content: flex-start | flex-end | center | space-between | space-around | 
    space-evenly | start | end | left | right ... + safe | unsafe;
  /* Using safe ensures that however you do this type of positioning, you can’t push an element such that it renders off-screen (e.g. off the top) in such a way the content can’t be scrolled too (called “data loss”). */

  align-items: stretch | flex-start/start/self-start | flex-end/end/self-end | center | baseline;
  /* stretch is default, will fill container | aligned to top | aligned to bottom | centered | aligned such as their baselines */
  /* also with safe and unsafe */

  /* this aligns the lines of the items if they are multiple */
  align-content: normal | flex-start | flex-end | center | space-between | space-around | space-evenly | stretch;
  /* with safe and unsafe */
}

.item {
  order: 5;
  /* default is 0 */

  flex-grow: 4;
  /* default is 0 */
  /* unitless value serves as proportion */

  flex-shrink: 3;

  flex-basis: 20% | 5rem | auto | content ...;

  flex: ;
  /* shorthand for flex-grow, flex-shrink and flex-basis */

  align-self: auto | flex-start | flex-end | center | baseline | stretch;
}
