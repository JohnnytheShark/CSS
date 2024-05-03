# Chapter 4 Creating a Responsive Web Newspaper Layout

## Set up basic Rules
You can import fonts from a CDN or third party using the 
@import url option in your css file.

rem = root em. An em is a relative unit based on the font size of the element's parent. Example: 
Parent Div has a font size of 12px then the child is set to .5em that would mean 12 x .5 = 6px. rem is based on the root element not the parent node. 

## Font-Weight Property: 

Font Weight is hold bold the lettering of the font is.

| Value    | Common Weight Name |
| -------- | ------- |
| 100 | Thin (Hairline)    |
| 200 | Extra Light (Ultra Light)   |
| 300 | Light  |
| 400 | Normal (Regular)|
| 500 | Medium |
| 600 | Semi Bold (Demi Bold) |
| 700 | Bold |
| 800 | Extra Bold (Ultra Bold) |
| 900 | Black (Heavy) |
| 950 | Extra Black (Ultra Black)  |

## Font Shorthand

Font Shorthand reads as: 
Font-Family Size Optionally: style, variant, weight, stretch, and line-height.
Syntax follows: font: font-style font-variant font-weight font-stretch font-size/line-height font-family

## Visual Hierarchy

Separate your data into groups by having different sizes for each of your headings

### Inline vs Block
Inline elements take up only the exact amount of space it needs for its content
Block create a new line and take the full width of their available space unless given a set width.


## CSS Counters
To create custom list style, we can use @counter-style at-rule
Example: @counter-style newListStyle {rules}
Then you would assign it to the list: ul { list-style: newListStyle;}