# Chapter 1 

Chapter 1 covers what CSS is and the order that CSS files are read on the browser. 

## Responsive Design: 

Single Fluid Layout that can change based on factors such as screen size, orientation, and device preferences. 

## Adaptive Design: 

Can also change based on these factors but it has multiple fixed layouts, which gives us greater control. Price to pay though is it takes more time than a singular responsive layout. 

## Order of CSS:

User-Agent Stylesheets: 
Browser Default Styles

Author Stylesheets:
Stylesheets that developers write.

User Stylesheets
User defined stylesheets, these are end users who override our existing styles. This is typically for users who need accessiblity changes. 


## Use of reset.css

Blank slate to start off with, resets all the styles that are inherited and gives us a great place to start from 

It's not ideal to have this as a separate file due to load times, and in production we would move the css at the beginning of the same file.

## Normalizer 

Instead of a using a reset.css option we could also use a css normalizer. 

Whether to use a reset.css or a normalizer.css is up to preference and not a necessity anymore. 

## Specifity Wins

When determining what will win out the larger number wins. 
Here is the breakdown of values: 
100 - ID selectors 
10 - Class Selectors,attribute selectors, and pseudo-classes
1 - Type selectors and pseudo-elements 
0 - universal selectors 

If there is a tie the browser looks at which stylesheet the style originated from. If both values come from the same stylesheet, the one later in the document wins. If they are on separate then:
1. User Stylesheet
2. Author Stylesheet (Order in which they are being imported; the last one wins)
3. UA Stylesheet

Separate rule: !important
Generally told not to use it as it breaks the flow, but can be used. Anything with this annotation wins out.


## Selecting Elements:
1. Type Selectors: think broader scale h1,h2,h3,p
2. Class Selectors: Different ways of building these look at BEM [BEM](https://en.bem.info),SMACSS [SMACCS](http://smacss.com),Block,Element
3. ID selector: Unique elements, given an ID tag use of (#)
4. Combinators: Descendant Combinator (space), child combinator (>), Adjacent Sibling Combinator (+), General Sibling Combinator(~)
5. Pseudo-Class and Pseduo-element selectors: added to as selector to target a specific state of the element (hovering), also :has() applies when the elment has at least one descendant that meets the selector specified inside the parenthesis. Pseduo-Element use a double colon (::). The purpose of pseudo-elements is to allow us to style a specific part of an element. 
6. Attribute value selectors: The attribute value selector looks for a specific attribute with the same value. 
7. 