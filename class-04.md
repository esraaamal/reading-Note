# Grid
When grid-column-start is used alone, the grid item by default will span exactly one column. However, we can extend the item across multiple columns by adding the **grid-column-end** property.

grid-column-start: 1;
grid-column-end: 4;

__________________________

**Instead of defining a grid item based on the start and end positions of the grid lines** , you can define it based on your desired column width using the span keyword. Keep in mind that span only works with positive values..
Typing both grid-column-start and grid-column-end every time can get tiring. Fortunately, grid-column is a shorthand property that can accept both values at once, separated by a slash.
#### For example:
 grid-column: 2 / 4; will set the grid item to start on the 2nd vertical grid line and end on the 4th grid line.


***One of the things that sets CSS grids apart from flexbox is that you can easily position items in two dimensions: columns and rows. grid-row-start works much like grid-column-start except along the vertical axis.***


If typing out both grid-column and grid-row is too much , there's yet another shorthand for that. grid-area accepts four values separated by slashes: grid-row-start, grid-column-start, grid-row-end, followed by grid-column-end.
One example of this would be grid-area: 1 / 1 / 3 / 6;.

If grid items aren't explicitly placed with grid-area, grid-column, grid-row, etc., they are automatically placed according to their order in the source code. We can override this using the order property, which is one of the advantages of grid over table-based layout.

***By default***, all grid items have an **order of 0**, but this can be set to any positive or negative value, similar to z-index.

Specifying a bunch of columns with identical widths can get tedious. Luckily there's a repeat function to help with that.
For example, we previously defined five 20% columns with the rule **grid-template-columns: 20% 20% 20% 20% 20%;**. This can be simplified as **grid-template-columns: repeat(5, 20%);**



Grid also introduces a new unit, the fractional fr. Each fr unit allocates one share of the available space. For example, if two elements are set to 1fr and 3fr respectively, the space is divided into 4 equal shares; the first element occupies 1/4 and the second element 3/4 of any leftover space.

![..](img/home1.png);
