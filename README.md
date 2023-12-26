# Puzzle Pixel Icons
A Collection of Pixel Art Icons... Originally Developed for Mega Puzzle 2024  

View the full collection of icons using the [Icon Catalogue](https://nouveaureece.github.io/Puzzle-Pixel-Icons/)


## Recommended Method
For a number of reasons including accessibility and stability, it is recommended that one use `<svg>` and `<use>` for SVG icons over icon fonts. (Learn more in ["Seriously, Don’t Use Icon Fonts"](https://cloudfour.com/thinks/seriously-dont-use-icon-fonts/) by Tyler Sticka)  

### Install
Copy the `icons.svg` file to your project directory (or, if you really have to, copy/paste its contents into your HTML file)

### Usage
Include the following HTML whenever using an icon, replacing with your desired icon from the [Icon Catalogue](https://nouveaureece.github.io/Puzzle-Pixel-Icons/): 
```
<svg role="img">
    <title>A rubber duck with its wings tucked against its body</title>
    <use xlink:href="icons.svg#ppi-duck">
</svg>
```
Including the `<title>` element will provide both `aria-label` and hover tooltip functionality (and is highly encouraged)! If the icon is decorative, be sure to include `aria-hidden="true"` on the `<svg>` element.

**Note:** it is not required that you include `role="img"` on your `<svg>` element. That being said, a squashed bug in WebKit (Safari, iOS, macOS) did prevent SVGs from being read as images at one point, and this was a solution to that issue.

## Alternate Method
### Install
If one choses to forgo the above method and use an "icon font" method, one can import the CSS by simply adding this `<link>` within the `<head>` section of an HTML file...
```
<link rel="stylesheet" href="https://nouveaureece.github.io/Puzzle-Pixel-Icons/pixel-icons.css">
```
... or in a CSS file with `@import`:
```
@import url("https://nouveaureece.github.io/Puzzle-Pixel-Icons/pixel-icons.css")
```
### Usage
Simply include an `<i>` tag which conforms to the proper `ppi-...` class. For example, this would display the check mark icon:
```
<i class="ppi-check"></i>
```


## Accessibility
It's a good idea to be as accessible as possible, so if you are using an icon for purely decorative reasons, be sure to include `aria-hidden="true"` on the tag. For example:
```
<!-- A button with a decorative icon -->
<a href="...">

    <svg role="img" aria-hidden="true">
        <use xlink:href="icons.svg#ppi-duck">
    </svg>

    Buy a Rubber Duck
</a>
```

## Acknowledgements
These icons were designed for use in the Luddy LLC Mega Puzzle 2024 at the Luddy School of Informatics, Computing, and Engineering at Indiana University, Bloomington  

Some CSS code for the icon font was inspired by [Bootstrap Icons](https://icons.getbootstrap.com/), which is licensed under the MIT License.  
