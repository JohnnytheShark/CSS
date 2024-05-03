# Summary Cards with Hover Interactions

Summary Cards are used for a range of purposes, whether that be showing a preview for a film, buying a property, previewing a news article.

## Fast Centering: 
Display: grid
place-items: center; 

This will accomplish centering your divs. 

## Media Queries
Use Media Queries to be able to switch card positioning to individual cards

## Background-clip
Background Clip is used to give text a background image. It gives headings a unique look

## Structure for cards
<section><div>Text Elements Here</div></section>
To have a background on the cards use background-image for the given section

## Grid Display Options
You can use min-content to only take up the space the element needs for that given option.

## Transitions
Before we start hiding elements we want to check if the device supports the hover interaction. You can do this with the media query @media (hover:hover) and also combine it with other options. 

You can select everything that you do not want visible by using the following *:not(element)
example:
main > section > div > *:not(h2)

When we want to reshow the element when hovering or focus we can use the pseduo-class: :focus-within
This pseudo-class allows u to apply styles conditionally based on whether a descendant of the element is currently in focus

Since the animation is occuring only once 
We can set the transition property for all animations as such: 
transition: all 700ms ease-in-out;

## Darker Screen
Play around with background colors sometimes having a darker screen will make the images pop out