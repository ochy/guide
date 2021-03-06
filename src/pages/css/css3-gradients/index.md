---
title: CSS3 Gradients
---
## CSS3 Gradients


CSS3 gradients let you display smooth transitions between two or more specified colors.

Earlier, you had to use images for these effects. However, by using CSS3 gradients you can reduce download time and bandwidth usage. In addition, elements with gradients look better when zoomed, because the gradient is generated by the browser.

CSS3 defines two types of gradients:

* Linear Gradients (goes down/up/left/right/diagonally)
* Radial Gradients (defined by their center)

### CSS3 Linear Gradients

To create a linear gradient you must define at least two color stops. Color stops are the colors you want to render smooth transitions among. You can also set a starting point and a direction (or an angle) along with the gradient effect.

#### Syntax
    background: linear-gradient(direction, color-stop1, color-stop2, ...);

##### Linear Gradient - Top to Bottom (this is default)
The following example shows a linear gradient that starts at the top. It starts red, transitioning to yellow:
![default-linear-gradient](https://i.imgur.com/2uGfleD.jpg)

#### Example
```
<!DOCTYPE html>
<html>
<head>
<style>
#grad1 {
    height: 200px;
    background: red; /* For browsers that do not support gradients */
    background: -webkit-linear-gradient(red, green); /* For Safari 5.1 to 6.0 */
    background: -o-linear-gradient(red, green); /* For Opera 11.1 to 12.0 */
    background: -moz-linear-gradient(red, green); /* For Firefox 3.6 to 15 */
    background: linear-gradient(red, green); /* Standard syntax (must be last) */
}
</style>
</head>
<body>

<h3>Linear Gradient - Top to Bottom</h3>
<p>This linear gradient starts at the top. It starts red, transitioning to yellow:</p>

<div id="grad1"></div>

<p><strong>Note:</strong> Internet Explorer 9 and earlier versions do not support gradients.</p>

</body>
</html>
```

![default-linear-gradient](https://i.imgur.com/CvtXCMd.jpg)

##### Linear Gradient - Left to Right
The following example shows a linear gradient that starts from the left. It starts red, transitioning to yellow:
![left-to-right](https://i.imgur.com/e4dRvZR.jpg)

#### Example

```
<!DOCTYPE html>
<html>
<head>
<style>
#grad1 {
    height: 200px;
    background: red; /* For browsers that do not support gradients */
    background: -webkit-linear-gradient(left, red , green); /* For Safari 5.1 to 6.0 */
    background: -o-linear-gradient(right, red, green); /* For Opera 11.1 to 12.0 */
    background: -moz-linear-gradient(right, red, green); /* For Firefox 3.6 to 15 */
    background: linear-gradient(to right, red , green); /* Standard syntax (must be last) */
}
</style>
</head>
<body>

<h3>Linear Gradient - Left to Right</h3>
<p>This linear gradient starts at the left. It starts red, transitioning to yellow:</p>

<div id="grad1"></div>

<p><strong>Note:</strong> Internet Explorer 9 and earlier versions do not support gradients.</p>

</body>
</html>
```

![left-to-right](https://i.imgur.com/k4FSyXz.jpg)

#### Linear Gradient - Diagonal

You can make a gradient diagonally by specifying both the horizontal and vertical starting positions.

The following example shows a linear gradient that starts at top left (and goes to bottom right). It starts red, transitioning to yellow:

![diagonal](https://i.imgur.com/YvtbUBH.jpg)

#### Example

```
<!DOCTYPE html>
<html>
<head>
<style>
#grad1 {
    height: 200px;
    background: red; /* For browsers that do not support gradients */
    background: -webkit-linear-gradient(left top, red, green); /* For Safari 5.1 to 6.0 */
    background: -o-linear-gradient(bottom right, red, green); /* For Opera 11.1 to 12.0 */
    background: -moz-linear-gradient(bottom right, red, green); /* For Firefox 3.6 to 15 */
    background: linear-gradient(to bottom right, red, green); /* Standard syntax (must be last) */
}
</style>
</head>
<body>

<h3>Linear Gradient - Diagonal</h3>
<p>This linear gradient starts at top left. It starts red, transitioning to yellow:</p>

<div id="grad1"></div>

<p><strong>Note:</strong> Internet Explorer 9 and earlier versions do not support gradients.</p>

</body>
</html>
```

![diagonal-exp](https://i.imgur.com/8gKRhAp.jpg)



#### More Information:
<!-- Please add any articles you think might be helpful to read before writing the article -->
[MDN Documentatiion](https://developer.mozilla.org/en-US/docs/Web/CSS/linear-gradient) || [w3schools](https://www.w3schools.com/css/css3_gradients.asp)