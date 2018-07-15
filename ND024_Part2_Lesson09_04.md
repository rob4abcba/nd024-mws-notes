# Lesson 9.4 Quiz: srcset Quiz

## From Udacity:

### srcset and sizes Quiz
I want to recap what you just learned about the image attributes srcset and sizes. This is a chance for you to take a closer look at the syntax of each attribute before trying them out on a real page in the next two quizzes.

In this quiz, you'll experiment with srcset, and in the next you'll add sizes to give the browser even more information.

### Syntax
There are two flavors of srcset, one using x to differentiate between device pixel ratios (DPR), and the other using w to describe the image's width.

### Reacting to Device Pixel Ratio
<img src="image_2x.jpg" srcset="image_2x.jpg 2x, image_1x.jpg 1x" alt="a cool image">
Set srcset equal to a comma separated string of filename multiplier pairs, where each multiplier must be an integer followed by an x.

For example, 1x represents 1x displays and 2x represents displays with twice the pixel density, like Apple's Retina displays.

The browser will download the image that best corresponds to its DPR .

Also, note that there's a src attribute as a fallback.

### Reacting to Image Width
<img src="image_200.jpg" srcset="image_200.jpg 200w, image_100.jpg 100w" alt="a cool image">
Set srcset equal to a comma separated string of filename widthDescriptor pairs, where each widthDescriptor is measured in pixels and must be an integer followed by a w. Here, the widthDescriptor gives the natural width of each image file, which enables the browser to choose the most appropriate image to request, depending on viewport size and DPR. (Without the widthDescriptor, the browser cannot know the width of an image without downloading it!)

Also, note that there's a src attribute as a fallback.

Ready to give it a shot? Click "Continue to Quiz" to try it out!

(Make sure you have installed the Udacity Feedback Chrome Extension for this quiz.)

### Start Quiz
Here's the site that needs some srcset!
High DPI Images for Variable Pixel Densities explains Device Pixel Ratio in detail: device-pixels-per-CSS-pixel is not quite the whole story! Make sure you have installed the Udacity Feedback Chrome Extension!

Here's a working solution

## From Michael Phan:

### Syntax:
Use the identifier `x` to identify DPR. Example:
`<img src="image_2x.jpg" srcset="image_2x.jpg 2x, image_1x.jpg 1x" alt="a cool image">`

Use the identifier `w` to identify width. Example:
`<img src="image_200.jpg" srcset="image_200.jpg 200w, image_100.jpg 100w" alt="a cool image">`

#### Quiz:

Use srcset to help the browser decide which image to display depending on the browser's width and display density. You should make your changes to the site linked in the instructor notes.

[Link to quiz](http://udacity.github.io/responsive-images/examples/srcsetAndSizes/index-quiz1.html).

<details>
<summary>Solution:</summary>
<p>

```
<img class="dpi" src="images/Den_Haag_2x.jpg" 
srcset="images/Den_Haag_1x.jpg 1x, 
images/Den_Haag_2x.jpg 2x" alt=" den=" haag="">

<img class="w" src="images/Australia_1280w.jpg" 
srcset="images/Australia_1280w.jpg 1280w, 
images/Australia_640w.jpg 640w" alt="Australia from Space">
```

</p>
</details>

- - -
Next up: [Quiz: srcset and sizes](ND024_Part2_Lesson09_05.md) or return to [Table Of Contents](./ND024_TableOfContents.md)
