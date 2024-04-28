# Chapter 2: Designing a layout using CSS Grid

A grid is a network of lines that cross to forma a series of squares and rectangles.

Advantage of using a grid over a css flexbox is that it allows us to divide a page into regions and create complex layouts with relative ease.


## Types of Grid: 
1. Grid - Used when we want the browswer to display the grid at block-level box. The grid takes the full width of the container and sets itself on a new line. 
2. Inline-Grid used when we want thegrid to be an inline-level box. The grid sets itself inline with the previous content, much like a <span>.

Block Level box says that element should use the entire horizontal space of its parent element. Inline elements can allow other inline elmeents to be on the same horizontal line depending on the remaining space. 

## Terms: 
Grid Lines: lines run horizontally and vertically, they're numbered starting from 1 in the top left corner. On the opposite side to the positive numbers are the negative numbers. 

Grid Tracks are the spaces between the grid lines. They're made up of columns and rows. 

Within each track are grid cells. A cell is the intersection between grid row and grid column

We can use the grid-template-columns, and grid-template-rows properties to layout the grid. 

repeat() in css is afunction that takes two values that are comma separated. 1st value is how many columns or rows to create, the second value is the sizing of each column or row.

minmax(min,max) function made up of two arguments: the minimum and maximum range of the grid track. Min Value needs to be smaller than the max value. Otherwise the browser ignores max and relies only on min.

Auto: When the keyword auto is used for the maximum value, it's treated the same as max-content keyword The row's or column's dimensions will be equal to the amoutn of room that the content within the row or column requires. The use of auto for headers and footers allows it to grow automatically.

fractions (fr) unique to Grid, tells the browser how much room an HTML element hsould have compared with other elements by distributing the leftover space after the minimums have been applied.

Implicit Grid: The automatic creation of extra grid cells is also known as implicit grid.

## Grid Template Areas
If we want to set an element explicitly on a particular row and column of our grid, we have two options. First we can use the line numbers and dictate the position of the child as follows: grid-column: 1/4. First number represents where the element starts , and the second represents where it ends.

Instead of using numbers though we can use the grid-template-areas to name areas. A grid area can be a single cell but if it's more than one cell the cells must create a rectangular shape with all cells of the same name being adjacent. you wouldn't be able to make an L shape for example.

(.) dot notation used to define a cell that we intend to keep empty because the cell doesn't have a name. Content can't be assigned to it. 

Remember that we need to assign the properties their grid names. use the grid-area tag.

## Gap Property
Gap property is shorthand for the row-gap and column-gap properties. by setting the row and column gaps, we're defining the gutters between rows and columns. Gutters is a term from print design, defining the gap between columns. Default value is 0px. Gap property refers to the space btween the tracks of the grid. To set space around the grid use padding and margin.

gap vs grid-gap: 
As css grid was being defined, the specification for this property was called the grid-gap property but now gap is recommended. Gap 1st value is row-gap, 2nd value: column-gap. If only one is declared it applies to both.


## Media Queries: 
Media queries are at-rules: they start with the @ symbol and define the condition under which the styles they contain should be applied. The use of media queries with grid-template-areas allows us to reconfigure our layout with minimal code. 


## Accessiblitiy considerations
W3 Grid Layout Module Recommendations states: 
    Authors must use order and grid-placement properties only for visual, not logical, reordering of content. Style sheets that use these features to perform logical reordering are non-conforming
