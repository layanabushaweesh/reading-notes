# CSS Grid
The CSS Grid Layout Module offers a grid-based layout system, with rows and columns, making it easier to design web pages without having to use floats and positioning.

CSS Grid Layout is the most powerful layout system available in CSS. It is a 2-dimensional system, meaning it can handle both columns and rows, unlike flexbox which is largely a 1-dimensional system.

* Content Properties

.content {
  grid-column-start: 1;
  grid-column-end: 4;  /* this will fill 3 squares */
  grid-column-end: span 2; /* this will give it width of two squares */

  grid-column: 1 / 4; /* this shorthand combines start / end */
  grid-column: 2 / span 3;

  /* grid-row being the same thing */
  grid-row: 3 / span 3;

  /* combined */
  grid-column: 2 / span 4;
  grid-row: 1 / span 5;

  /* shorthand */
  /* grid-area: row-start / column-start / row-end / column-end */
  grid-area: 1 / 2 / span 3 / span 4;

  /* z-index equivalent */
  /* usually, highest order goes to end, similar to an array index */
  order: 1;
}


* Container Properties

.container {
  display: grid;
  grid-template-columns: 20% 20% 20% 20% 20%;
  grid-template-rows: 20% 20% 20% 20% 20%;
  /* this will make a five-by-five grid */

  /* similar to */
  grid-template-columns: repeat(5, 20%);
  grid-template-rows: repeat(5, 20%);

  /* various units may be used */
  grid-template-columns: 100px 3em 40%; /* three different sized columns */

  /* fractions */
  grid-template-columns: 1fr 5fr; /* first column occupying 1sixth, the second occupying 5sixths */

  /* combinations */
  grid-template-columns: 50px 1fr 1fr 1fr 50px; /* first and last column 50px each, with three equal columns in the middle */

  /* shorthand */
  /* grid-template: rows / columns */

}