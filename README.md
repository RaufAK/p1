# Project 1 
Style sheet C: Added the two animations to p1.html 
and also created the styleC.css  file and 
added the gradient background as well as a svg animation with the text.

The SVG:The code in p1.html starts with the animation viewBox, this is an attribute that specifies the coordinate system of the SVG content.
Inside the <symbol>, there are two <text> elements that define text elements. They are positioned with x and y attributes,
and text-anchor is set to "middle" to horizontally center the text
<g> is a grouping element that can be used to group the SVG elements together.
class="g-ants" assigns a class name to this <g> element.
Inside the <g> element, there are five <use> elements. These <use> elements reference the symbol with the xlink:href attribute, 
and the referenced symbol is "s-text." Each <use> element duplicates the content of the "s-text" symbol.
class="text-copy" is assigned to each <use> element.

The CSS: SVG .text-copy is a CSS class selector applied to multiple elements.
fill: none; specifies that the text elements should not have a fill.
stroke: #FDFFFC; sets the stroke color of the text elements to a light color (#FDFFFC).
stroke-dasharray: 6% 29%; defines a pattern for the dashed stroke. It creates a dash pattern where the dashes are 6% of the path length, and the gaps between dashes are 29% of the path length.
stroke-width: 5px; sets the width of the stroke lines to 5 pixels.
stroke-dashoffset: 0%; sets the initial position of the stroke dash offset to 0%, meaning the dashes are initially aligned with the path.
animation: stroke-offset 5.5s infinite linear;animation-delay is used to stagger the start of the animation for each text element. Negative values like -1s, are used to create the stagger effect.
@keyframes defines a custom animation named stroke-offset.
Inside the keyframes, stroke-dashoffset is animated from its initial value of 0% to its final value of -35%.
This animation creates the effect of the dashed strokes moving along the path.

Some useful Links that helped me get here:https://developer.mozilla.org/en-US/docs/Web/SVG/Element/textPath
https://alvarotrigo.com/blog/css-text-animations/
https://developer.mozilla.org/en-US/docs/Web/SVG/Tutorial/Paths
