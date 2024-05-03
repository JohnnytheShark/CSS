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

## Photo Filters
We can use the filter property to add a filter to our images. Filters can impact load speed so use them wisely. 

Handling broken image links: 
Add alt text to display when an image is unable to be displayed.

You can add an onerror Javascript event handler to trigger a change in styles as follow: 
<img src"..." alt="..." onerror="this.style.display='none'">
This will remove the image altogether

We can also add a caption to the image using <figure> and <figcaption>

## CSS Multi-Column Layout Module
This is a lesser known way of laying things out compared to grid and flexbox. The purpose is to allow content to flow naturally between multiple columns. column-count: number; under a section to implement it.

You can add column-rule which adds a solid border
To adjust spacing using column-gap

### Media Query
Is a type of at-rule; to set up new rules based on screen size. 

### Gestalt Design Principles: 
The prinicples are a collection of principles of human perception that describe how humans group similar elements.

Principles go as followed: 
1. Similarity - Shared Visual Characteristics automatically create relationships. Similarity can be used to tie together elements that may not be right next to each other in design.
2. Continuation - The principle of continuity posits that the human eye will follow the smoothest path when following something, and it will continue travelling in that direction until it encounters another object.
3. Closure - Is the ideas that the brain will fill in the missing parts of an image to create a whole. As long as enough essential information is present. THe mind supplies the missing pieces of an object
4. Proximity - Referes to objects that are close together being perceived as a group. When placed apart, objects are seen as separate. Proximity arises when objects are closer to each other than to any other object. 
5. Figure/Ground - The F/G principle is based on the relationship between an object and the surrounding space. It also refers to positive and negative space, the positive being the object and the negative being the space.
6. Symmetry and Order (Pragnanz) - The law of symmetry and order is also known as pragnanz. The german word for good figure. What this principle says is taht the brain will perceive ambiguous shapes in as simple a manner as possible. 
7. Synchrony (Common Fate) - Not originally included but has since been added. People will group things together that point to or are moving in the same direction.

### Making objects span multiple columns: 
You can use column-span: all to do so.

### Prevent Images and Captions from being separated: 
Use break-inside: avoid property.

### Justifying Paragraph Text: 
Text-align: justify. 
Also you can adjust hyphenation with: hyphens: auto;

### Wrapping Text around Images: 
You can add the float property to the figure to cause the text to be wrap. Float pushes it to the left or right allowing inline elements to wrap around 

### Handling Super Wide Screens: 
