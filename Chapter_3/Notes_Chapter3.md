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

Keyframes are described as @keyframes in this secenerio we create different animation styles based on the keyframe type. Example @keyframes changeColor{
    0% {background: blue}
    50% {background: yellow}
    100%{background: red}
}

In this scenerio the animation is changing colors from blue to yellow to finally red

### Animation Parts: 
Duration: The duration property sets how long we want the animation to happen from start to finish. The duration can be set in seconds (s) or milliseconds (ms). The longer the duration, the more slowly the animation completes. With accessibility in mind we want to consider users who are sensitive to motion and choose a duration that is reasonable. 

Remember to not have flashes more than three times in any 1 second period to reduce seizures. 

Iteration Count: Sets how many times the animation should repeat. Default is 1. You can always set it to infinite (but remember this will go on for eternity)

Animation shorthand: 
animation: animation-name animation-duration animation-iteration-count

You can add animation-delay to elements that are animated to help get new effects.

Transform-Origin:
Property sets the origin, or the point, for an element's transformations. If we were to rotate tthe object, the transform-origin property would set where the on the element we want to rotate from.

## Accessibility and prefers-reduced-motion media query

To respect users that have sensitivities to motion this query was introduced. You can turn off animation on your site if need be through this.

## Styling HTML Progress Bar
HTML Progress bar allows us to show our users where in the process our process is at. 
Progress bars need a vendor prefix to work correctly: 
-webkit- Chrome, Safari, Opera, Edge
-moz- Firefox





