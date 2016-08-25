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

## Chapter 4 - Other CSS classes


1. Buttons
class="btn btn-default": for <a>, <button>, <input>
Only <button> works within <nav>, or things with role="button", which is less obvious than simply using a button.
btn-color: default, primary, success, info, danger
btn-size: default, lg, sm, xs and block (to take the full line)
"active" class
"disabled" class

2. Tables
class="table": makes it look great.
class="table-striped": did not work out.
table-bordered
table-hover: did not work either
table-condensed: less padding;
classes: active, success, info, warning, danger: color
div class="table-responsive": adds vertical scrolling after a certain breakpoint

3. Image Classes
Class "img-responsive": sets image max-width to 100%; sets height to auto and element to block;
center-block: centralizes any block
I can edit the .img-responsive class through css, of course.
Class "img-rounded": rounded edges, look pretty good
"img-circles", "img-thumbnail": super useful!

4. Helper/Miscellaneous classes
p:
text-muted: text-color a little lighter
text- primary, success, info, warning, danger: a little darker than in other classes, so that the text is readable
bg- primary, success, info, warning, danger
img:
pull-left and pull-right: quick float; they don't work for navigation elements
center-block
also... for anything, specially used in JS:
show
hidden
invisible (transparency set to 0, but still takes space)
sr-only: only shows something on a screen reader
sr-only-focusable
text-hide: hide texts, assuming you're replacing it for an image

5. Responsive utilities
VISIBILITY-SIZE(-DISPLAY)
visibility: visible or hidden
size: xs, sm, md, lg, *print*
display: block, inline, inline-block, print

### Chapter 5 - Forms

1. Basic form
Labels: tapping on labels activate elements; screen-readers.
ID="inputEmail": mobile phones identify it. probably auto-filling.
Label class="sr-only" only shows up on screen-readers.
*class="form-control": padding, color, highlight, spacing, 100% width. *
div class="form-group": separates  labels and inputs among themselves.
div class="checkbox"
button class="pull-right"

2. Radio and checkbox
Div class="checkbox": labels are wrapped with the input; does not need "for" attribute.
Checkboxes: one and/or more options.
Class radio-inline: side-by-side. Should be within a form-group div to not mix with following inputs.

3. Inline forms
Horizontal
<form class="form-inline">
sr-only class to hide labels
Useful for short forms (not many inputs), like search and login forms.

4. Horizontal form
Great for mobile, 'cause labels are usually hidden when tapped into input field.
class="control-label": adjusts label to input beautifully
On mobile devices, labels are placed on top of fields. That's pretty cool!

5. Validation styles
class= "has-warning", "has-error", "has-success"
works well with "control-label", so that the label also gets the color
add class="has-feedback"
<span class="glyphicon glyphicon-ok form-control-feedback">
260 halflings at glyphicons.com
aria-hidden="true": not visible on screen-readers.
(Lesson does not explain how to activate the success id based on user's input)

6. Input groups
<span class="input-group-addon">Label</span> within div class="input-group"
Works at the beginning or at the end.
Aria-label: label for screen-readers.
Accessible Rich Internet Application (ARIA)
Placeholder: not the "value", but an information that is just visually shown.
<span class="input-group-btn">: an input group, with text inside
*Nice lesson!*

7. Styles and sizing
"disabled" attribute/class: changes style and cursor
<fieldset><legend>Basic Info</legend><input ...> ... </fieldset>
"readonly" attribute: initial value cannot be changed
"form-control-static" class: makes paragraphs align like inputs.
classes input-SIZE and form-group-SIZE, like input-lg, input-sm, ... 


8. Icons
<span class="glyphicon glyphicon-print"></span>, with nothing inside.
Adjusts to the size of outer tag, like an inline size (within a P) or any Header# size.
Using <i> (icon tag) is a little controversial. Preferably, span tag.
add aria-hidden="true" to span, so that screen readers do not read it.
Works well within buttons as well. Add aria-label to it, if there is no text with it.

### Chapter 6 - Navigation Components


1. Dropdown
div class="dropdown"
data-toggle="dropdown"
*Best lesson so far...*
<div class="dropdown">
<div class="btn-group">
<button type="button" class="btn btn-info">Search Pet Info</button>
<button type="button" id="pettype" aria-haspopup="true" aria-expanded="false"
  class="btn btn-info dropdown-toggle" data-toggle="dropdown">
  <span class="caret"></span>
  <span class="sr-only">Toggle Dropdown</span>
  </button>

<ul class="dropdown-menu" aria-labeldby="pettype">
  <li class="dropdown-header">Common</li>
  <li><a href="#">Cat</a></li>
  <li><a href="#">Dog</a></li>
  <li><a href="#">Fish</a></li>
  <li role="separator" class="divider"></li>
  <li class="disabled"><a href="#">Birds</a></li>
  <li><a href="#">Amphibian</a></li>
  <li><a href="#">Reptile</a></li>
  <li><a href="#">Other</a></li>
</ul>
</div>
</div>

2. Button groups
div class="btn-group": unifies buttons; can be button-group-vertical as well.
role="group": adding roles to tags makes screen-readers identify their functionality.
labels, on the other hand, makes screen-readers know what to say.
aria-label="..."
btn-group within btn-group for each button makes buttons take 100% width.

3. Bootstrap nav
ul class="nav" nav-tabs, nav-pills, nav-stacked, nav-justified
li class="active" (active tab)
li role="presentation", if not within <nav></nav>
Usually within <nav> outside containers, on top of body.
<nav class="navbar navbar-default">, 
or navbar-inverse (black background)
or navbar-fixed-bottom, navbar-fixed-top
Use inspect element to know how to stylize it.

4. Navbar
Brand: any text or icon. Class navbar-brand, goes within navbar-header.
<p class="navbar-text">A speak-first approach to language learning.</p>
navbar-left, navbar-right (for Search, for example): essentially, a float attribute.
button class="navbar-btn": button within navbar, aligned properly.

5. Collapsing navigation
Hamburger menu

<nav class="navbar navbar-default">
  <div class="container">
    <div class="navbar-header">
      <button type="button" class="navbar-toggle collapsed" data-toggle="collapse" data-target="#collapsemenu"  aria-expanded="false">
        <span class="sr-only">Toggle navigation</span>
        <span class="icon-bar"></span>
        <span class="icon-bar"></span>
        <span class="icon-bar"></span>
      </button>
      <a href="#" class="navbar-brand">
        Wisdom Pets
      </a>
    </div>
<div class="collapse navbar-collapse" id="collapsemenu">
    <ul class="nav navbar-nav">
      <li><a href="#">Home</a></li>
      <li class="active"><a href="#">Mission</a></li>
      <li><a href="#">Services</a></li>
      <li><a href="#">Staff</a></li>
      <li><a href="#">Testimonials</a></li>
    </ul>    
</div>


6. Breadcrumbs / Pagination
ul class="breadcrumb"
(doesn't explain how to set it up properly, it's just a style class)
pagination:
<nav>
<ul class="pager">
  <li class="previous"><a href="#"><span aria-hidden="true">&larr;</span> Older</a></li>
  <li class="next"><a href="#"><span aria-hidden="true">&rarr;</span> Newer</a></li>
</ul>
</nav>

### Chapter 7 - Media Components

