Tutorial
--------
<pre> 
<h3>Grid Layout</h3>
The CSS Grid Layout Module offers a grid-based layout system, with rows and columns, making it easier to design web pages without having to use floats and positioning.
<h4>Grid Elements</h4>
A grid layout consists of a parent element, with one or more child elements.
<br>
Example:
    &ltdiv class="grid-container"&gt; - parent element
        &ltdiv class="grid-item"&gt; 1 &lt/div&gt; - child element
        &ltdiv class="grid-item"&gt; 2 &lt/div&gt; - child element
    &ltdiv&gt;
 
<h4>Display Property</h4>
An HTML element becomes a grid container by setting the display property to grid or inline-grid.
Example:
    .grid-container {
         display: grid;
    }
    .grid-container {
        display: inline-grid;
    }
All direct children of the grid container automatically become grid items.

<h4>Grid Columns, Rows, Gaps</h4>
The vertical line of grid items are called columns.
The horizontal line of grid items are called rows.
The space between each column/row are called gaps.

You can adjust the gap size by using one of the following properties:
    grid-column-gap
    grid-row-gap
    grid-gap
    
Example:
The grid-column-gap property sets the gap between the columns:
    .grid-container {
          display: grid;
          grid-column-gap: 50px;
    }
The grid-row-gap property sets the gap between the rows:
    .grid-container {
          display: grid;
          grid-row-gap: 50px;
    }
The grid-gap property is a shorthand property for the grid-column-gap and the grid-row-gap properties:
    .grid-container {
         display: grid;
         grid-gap: 50px 100px;
    }
The grid-gap property can also be used to set both the row gap and the column gap in one value:
    .grid-container {
         display: grid;
         grid-gap: 50px;
    }

<h4>Grid Lines</h4>
The line between columns are called column lines.
The line between rows are called row lines.
Refer to line numbers when placing a grid item in a grid container:
Example
Place a grid item at column line 1, and let it end on column line 3:
    .item1 {
         grid-column-start: 1;
          grid-column-end: 3;
    }
Place a grid item at row line 1, and let it end on row line 3:
    .item1 {
          grid-row-start: 1;
          grid-row-end: 3;
    }
