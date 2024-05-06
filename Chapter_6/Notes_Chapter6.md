# Creating Profile Card

## Setting CSS custom properties
To create a custom property, we prefix the variadble name with two hyphens (--) immediately followed by the variable name. We assign the value to a custom property the same way that we do any other property: with a colon (:) followed by the value. A CSS variable declaration, therefore, looks like this: --variableName: value;

Example of usage: 
--page-background: linear-gradient(#4F5D75, #2D3142)
background: var(--page-background);

## Linear Gradient
A linear gradient is a type of image. When we apply an image as a background to an element in CSS, if the image is smaller than the elemenet the image will repeat (tile).

## Flex Box
To center the card in the exact middle of the screen we can use flexbox

Display: flex;
To center horizontally we add justify-content: center 
To center vertically we add align-items: center

## Styling Image
object-fit: cover sets the image to maintain its initial aspect ratio but fit itself to fill the space available. In this case, we'll lose a little of the top and bottom of the image due to the image being taller than it is wide. 

Making a circle image set the border-radius to 50% and insure width and height are set to a square

To have a image stick above the card we use a negative margin. 

## Rem
A rem is a relative unit based on the font size of the root element

## DL
<dl> is a description list
<dt> Title
<dd> is the value

## Flex Basis and Flex Shrink
Flex-basis sets the initial size the browser should use when calculating the amount of space an element needs. 

Flex-shrink dictates whether an element is allowed to shrink smaller than the size assigned by the flex-basiss value if there's not enough room for the element in the container. If the flex-shrink value is 0, the size isn't adjusted. Any positive value allows for resizing. 

## Classes can be accessed through dot notation 
p.summary is something new but will work for all paragraphs with a class of summary