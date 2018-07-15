# Lesson 9.5 Quiz: srcset and sizes

## From Udacity:

### Image Width with sizes
What if the image won't be displayed at the full viewport width? Then you need something more than srcset, which assumes the image will be full viewport width.

Add a sizes attribute to the image with a media query and a vw value. srcset and sizes together tell the browser the natural width of the image, and how wide the image will be displayed relative to viewport width. Knowing the display width of the image and the widths of the image files available to it, the browser has the information it needs to download the image with the right resolution for its needs that is as small as possible. And it can make this choice early in the page load while the HTML is still being parsed.

### srcset with sizes Syntax
Here's an example:

<img  src="images/great_pic_800.jpg"
      sizes="(max-width: 400px) 100vw, (min-width: 401px) 50vw"
      srcset="images/great_pic_400.jpg 400w, images/great_pic_800.jpg 800w"
      alt="great picture">
sizes consists of comma separated mediaQuery width pairs. sizes tells the browser early in the load process that the image will be displayed at some width when the mediaQuery is hit.

In fact, if sizes is missing, the browser defaults sizes to 100vw, meaning that it expects the image will display at the full viewport width.

sizes gives the browser one more piece of information to ensure that it downloads the right image file based on the eventual display width of the image. Just to be clear, it does not actually resize the image - that's what CSS does.

In this example, the browser knows that the image will be full viewport width if the browser's viewport is 400px wide or less, and half viewport width if greater than 400px. It knows that it has two image options - one with a natural width of 400px and the other 800px.

Ready to help the browser out? Click "Continue to Quiz" to try it yourself!

(Make sure you have installed the Udacity Feedback Chrome Extension for this quiz.)

### Start Quiz
Here's the site that needs some srcset and sizes!
A word about how w units work, from Yoav Weiss who implemented responsive images for Chrome and other browsers:

The selection logic is not defined in the spec (on purpose) so that every browser can apply their own selection logic, and be able to optimize the selected resources over time, in order to achieve the best quality/byte-size tradeoff for their users.

Blink's current selection logic Blink is the rendering engine used by Chrome is based on a geometric mean of adjacent (sorted by density) resource candidates.

If the DPR is a value between the densities of two adjacent candidates, the browser calculates the candidates' geometric mean. If DPR is higher than the geo mean, the candidate with the larger density value "wins". Otherwise, it's the smaller one.

For your example, the geo mean of 500w and 1000w is 707, which explains why only above that value, the larger resource gets picked. Make sure you have installed the Udacity Feedback Chrome Extension!

Here's a working solution
Have questions? Head to the forums for discussion with the Udacity Community




## From Michael Phan:

### Example code with srcset and sizes syntax:
```
<img  src="images/great_pic_800.jpg"
      sizes="(max-width: 400px) 100vw, (min-width: 401px) 50vw"
      srcset="images/great_pic_400.jpg 400w, images/great_pic_800.jpg 800w"
      alt="great picture">
```
#### Quiz:
[Link to quiz](http://udacity.github.io/responsive-images/examples/srcsetAndSizes/index-quiz2.html).

Use srcset and sizes to help the browser decide which image to display when the image is displayed at less than the full viewport width. You should make your changes to the site linked in the instructor notes.

<details>
<summary>Solution:</summary>
<p>

```
<img class="w" src="images/Coffee_1280w.jpg" 
sizes="(max-width: 960px) 50vw, 100vw" 
srcset="images/Coffee_1280w.jpg 1280w, images/Coffee_640w.jpg 640w" 
alt="Coffee by Amy March from Turkey">
```

</p>
</details>

- - -
Next up: [The Picture Element](ND024_Part2_Lesson09_06.md) or return to [Table Of Contents](./ND024_TableOfContents.md)
