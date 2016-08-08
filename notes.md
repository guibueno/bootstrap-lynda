## Chapter 2 - Grid

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

## Chapter 3 - Basic Bootstrap classes

1.
Emulate Headlines through classes H1-H6
There is a style for <small> within <h_>
Class "small" also exists
Every paragraph has a 10px margin-bottom originally.
Class "lead" for text that need to stand out
These utility classes are all customizable.

2. Inline Text Styles: NOTHING new. Just that Bootstrap changes browser defaults for in-line elements.
<mark>: light yellow bg, black text. It overwright the default class from the browser.
<s> and <del>: semantic difference. <ins> for text that has been inserted.
<small>: font-size is smaller in around 85 percnt.

3.Alignment, transformation, abbreviations
Classes "text-left", "text-right", "text-center", "text-justify"... "text-nowrap": endless line, without breaking.
Classes "text-lowercase", "text-uppercase", "text-capitalize"
<abbr title="Captain">Capt.</abbr>: question mark icon is added by bootstrap
<abbr title="Federative Republic of Brazil" class="initialism">FRofB</abbr>: uppercase, smaller font 

4. Blockquotes
Add within blockquote: <footer>Person the quote is from</footer>: stylizes and adds dash.
class="blockquote-reverse" aligns to the right.

5. Lists
class "list-unstyled": only affects one of the levels; takes off all style.
class "list-inline": gets rid of bullets and puts items side by side.
class "dl-horizontal": for dictionary entries. Really nice looking!

6. Code
<code>
<kbd>: Keyboard Tag, for shortcuts. Looks nice!
<var>: help search engines by identifying variables.
<pre>: Pre-formatted text. Nice-looking box!
<samp>: Like <pre>, but without the box. Sample output tag.
<pre class="pre-scrollable">: Long code. Scrollable. 300px