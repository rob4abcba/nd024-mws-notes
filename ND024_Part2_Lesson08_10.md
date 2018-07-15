# Lesson 8.10 Quiz: Strategy Quiz 1


Tere are a Few different techniques for handling images
external files link in your HTML
inline image with all data right in your page
raster star element
Use vector images like this star from material design
Use font icons like "Font Awesome" then Use CSS techniques for styling them.

Many different techniques all get the Same result
The "right" strategy depends on the image's place in the app as a whole

Here's a Scenario for a mobile app that posts Bikes For Sale.
Want to put an image for a star at the upper right corner to indicate bikes which got put on sale within the past 24hrs

Scale the star 

Which options for the star are best?  Should you:
Q1: vector or raster graphic?
Q2: inline the icon or set its source to an external file?

Solution:
S1: Star is simple and regular shape, so vector graphic is better and is good for scaling with your app
S2: Could argue either inline image or set its source to an external file.  
--inline star simple can create with SVG.  inline not add many bytes.
--If re-use image, then external file  <--  can cache and not have to reload every time
so both inline an external are ok
Test it to find out which method is faster.

- - -
Next up: [Quiz: Strategy Quiz 2](ND024_Part2_Lesson08_11.md) or return to [Table Of Contents](./ND024_TableOfContents.md)
