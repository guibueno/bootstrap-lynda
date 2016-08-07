Chapter 2 - Grid

Containers have 15px padding.

12 columns

Fluid and Fixed containers.
Fluid adjusts.
Fixed-width: adjusts to media query breakpoints; breakpoints

Rows: prepare containers for having columns
placed inside containers;
should always use columns;
gets rid of container padding (through negative margin)

Columns: 
30px gutters (calha): 15px on each side
col-SIZE-SPAN
SIZE: when it stacks
when it converts to full width column
xs, sm, md, lg
SPAN: number of columns (out of 12)

Sections and Divs may use Bootstrap classes. Maybe anything.

Tags may have 2 classes, therefore 2 breakpoints for different browser sizes.

Clearfix class: clears problems with floats.
visible-sm-block
hidden-sm-inline
Used to fix layout problems, column problems
Also used to hide or make visible things at certain browser sizes


Block elements take over all the columns

Offset: like a "margin"ish column space before the element.
It can potentially affect other breakpoints.
We need to make sure we reset them, as a consequence.

Rows inside other rows. 12 grid inside 12 grids.
Nested rows.

Push and pull
col-xs-push-1