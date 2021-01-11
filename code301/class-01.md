# Responsive Web Design and Floats

## Responsive Web Design
### Overview
  - Practice of buildings a website that works on every device and screen size.
  - created by Ethan Marcotte
  - 3 main components
    - flexible layouts
    - media queries
    - flexible media
### Responsive vs Adaptive vs Mobile
  - responsive means to react quickly and positively to change
  - adaptive means to easily modify for new purpose or situations
  - movile means to create a website on a new domain for mobile users
### Flexible Layouts
  - practice of buildings layout of website with flexible grid
  - capable of dynamically resizing to any width
  - Relative length units ems or %
  - width, margin or padding
#### Relative Viewport Lengths
  - vw Viewports Width
  - vmin Minimum of the viewports height and width
  - vh Viewports height
  - vmax Maximum of the viewports height and width
#### Flexible Grid
```
section,
aside {
  margin: 1.858736059%; /*  10px ÷ 538px = .018587361 */
}
section {
  float: left;
  width: 63.197026%;    /* 340px ÷ 538px = .63197026 */   
}
aside {
  float: right;
  width: 29.3680297%;  /* 158px ÷ 538px = .293680297 */
}
```

### Media Queries
  - built as an extension to media types found when targeting and including styles
  - can specify different styles for each browser and device
  - uniquely apply targested styles
#### Initializing Media Queries
  - @media rule used inside style sheet
  - @import brings in a new style sheet
```
/* @media Rule */
@media all and (max-width: 1024px) {...}

/* @import Rule */
@import url(styles.css) all and (max-width: 1024px) {...}
```
  - linking to a seperate style sheet in the html document
  ```
  <link href="styles.css" rel="stylesheet" media="all and (max-width: 1024px)">
  ```

#### Common Media Types

  - all
  - screen
  - print
  - tv
  - braille

#### Logical Operators in Media Queries
  - 3 different logical operators
    - and logical operator allows an extra condition to be added

    ```
    <link href="styles.css" rel="stylesheet" media="all and (max-width: 1024px)">
    ```
    - not logical operator negates the query, specifying any query but the one identified

    ```
    @media not screen and (color) {...}
    ```
    - only logical operator selects only screens in portrait with user agent capable of rending media queries

    ```
    @media only screen and (orientation: portrait) {...}
    ```

  #### Media Features in Media Queries

-  Identify what attributes or properties will be targeted within expression

    - Height
      - min
      - max
    - Width
      - min
      - max

```
@media all and (min-width: 320px) and (max-width: 780px) {...}
```

#### Orientation Media Feature
- landscape
- portrait

```
@media all and (orientation: landscape) {...}
```
#### Aspect Ratio Media Features
- specifies width/height pixel ratio
  - aspect-ratio
  - device-aspect-ratio

```
@media all and (min-device-aspect-ratio: 16/9) {...}
```
#### Resolution Media Feature
- specifies resolution of output device in pixel density, dots per inch or DPO

```
@media print and (min-resolution: 300dpi) {...}
```

#### Other Media Features
- color
- color-index
- monochrome
- grid
- scan

### Mobile First
  - Use smaller viewport styles as default for website, then use media queries as it grows
  - smaller viewport shouldnt have to load styles for desktop
  - saves bandwith
  - constraints of mobile user in mind

```
/* Default styles first then media queries */
@media screen and (min-width: 400px)  {...}
@media screen and (min-width: 600px)  {...}
@media screen and (min-width: 1000px) {...}
@media screen and (min-width: 1400px) {...}
```

#### Viewport
- invented by apple
- height
  - device-height
- width
  - device-width
- scale
  - initial-scale
  - user-scalable
  - minimum-scale
  - maximum-scale
- Viewport Resolution
  - target-densitydpi
  - device-dpi
  - high-dpi
  - medium-dpi
  - low-dpi
  - dpi number

### Flexible Media
- media size changes with viewport
  - max-width

```
img, video, canvas {
  max-width: 100%;
}
```

- Flexible Embedded Media
  - absolutely positioned inside parent

```
HTML
<figure>
  <iframe src="https://www.youtube.com/embed/4Fqg43ozz7A"></iframe>
</figure>

              
CSS
figure {
  height: 0;
  padding-bottom: 56.25%; /* 16:9 */
  position: relative;
  width: 100%;
}
iframe {
  height: 100%;
  left: 0;
  position: absolute;
  top: 0;
  width: 100%;
}
```

## Floats
- CSS positioning property
- text wraps
- float properties
  - left
  - right
  - none
  - Inherit
- clear - floats sister property
  - will not move up adjacent to float
  - will move down past float
  - 4 valid values
    - Both
    - Left
    - Right
    - None
  - Empy Div Method
  - Overflow Method
  - Easy Clearing Method
    - `:after`
- fragile



[Home](../README.md)