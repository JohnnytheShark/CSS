# Creating responsive animated Loading Screen

## Elements to be used: 
HTML <progress> element and svgs

## SVG Basics
SVG stands for scalable vector graphics. SVGS are written in an XML-based markup language and consist of vectors on a Cartesian Plane.

Vector: Mathematical formula that creates lines, polygons, curves, circles, and rectangles, along with other geometric preimitives. 

Cartesian coordinate system is a grid based system that defines a point by using a pair of numerical coordinates based on the point's distance from two perpendicular axes. 

Advantages:
Scalability, written in XML can be access, manipulated, and edit in the same way we do with other html elements. 


Origin (0,0) starts in top left corner 

SVG Viewbox sets the position, height, and width of the graphic within the viewport. 

## Shapes in SVG
rect (rectangle)
circle
ellipse
line
polyline
polygon

Irregular shapes can be created with path. 

## Animations
animation-delay: How long to wait before the animation starts
animation-direction- Whether the animation is played forward or backward
animation-duration - How long it should take for the animation to run once
animation-fill-mode - How the elmeent being animated should be styled when the animation is done executing
animation-iteration-count - How many times the animation should run
animation-name: Name of the keyframes being applied
animation-play-state - Whether the animation is running or paused
animation-timing-function - how the animation progresses through the styling over time 

Keyframes are described as @keyframes