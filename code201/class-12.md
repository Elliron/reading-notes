# Charts
Better at displaying data visually than tables

Import script

```
<!DOCTYPE html>
<html lang="en">
  <head>
    <metacharset="utf-8">
    <title>Chart.js demo</title>
    <script src='chart.min.js'></script>
  </head>
  <body>
  </body>
</html>
```

Line Chart
add to html body

```
<canvas id="buyers" width="600" height="400"></canvas>
```

add foot to body element

```
<script>
  var buyers = document.getElementById('buyers').getcontext('2d');
    new Chart(buyers).Line(buyerData);
</script>
```
create data

```
var buyerData = {
  labels : ["Jan", "Feb", "March"],
  datasets L [
    {
      fillColor : "rgba(123,432,523,0.2)",
      strokeColor : "#ACC26D"
      pointColor : "#fff",
      pointStrokeColor : "#9dB86D"
      data : [203, 156,99]
    }
  ]
}
```

## Pie Chart

Create Data

```
var pieData =[
  {
    value : 20,
    color : "#878BB6"
  },
  {
    value : 40,
    color :  "#4ACAB4"
  }
];
```
pie options

```
var pieOptions = {
  segmentShowStroke : false,
  animateScale: true
}
```

Bar Chart

Create Data

```
var barData = {
  labels: ["Jan", "Feb", "etc"]
  datasets : [
     {
       fillColor : "#32AD4324",
       strokeColor : "#",
       data L [ 345, 234, etc]
     },
     {
        fillColor : "#32AD4324",
       strokeColor : "#",
       data L [ 345, 234, etc]
     }
  ]
}
```

## Basic Usage

**Canvas Element** 300pxx150px default
  - width
  - height
  - fallback content
  - **rendering contexts** create and manipulate content shown

## Drawing shapes with canvas

  - **coordinate space** or grid, 1 unit of grid corresponds to 1 px on canvas.  origin is positioned in the top left corner at `(0,0)`.

  ### rectangles
  - draw and fill  `fillRect(x, y, width, height)`

  - draw and outline ` strokeRect(x, y, width, height)`
   - clear and make transparent ` clearRect(x, y, width, height)`

### Drawing 

- `beginPath()` creates a new path
- Path methods methods to set different paths for objects
- `closePath()` adds straight line to path, start of current sub-path
- `stroke()` Draws shape by stroking outline
- `fill()` draws solid shape by filling paths content area

### Moving pen
- `moveTo(x, y)` moves the pen to specified coordinates

### lines
- `lineTo(x, y)` draws line from current position to specified position

### Arcs
`arc(x, y, radius, startAngle, endAngle, anticlockwise)` draws an arc centered at (x, y)
- `arcTo(x1, y1, x2, y2, radius)` draws an arc with given control points and radius connected to previous point

Bezier and quadratic curves
- `quadraticCurveTo(cp1x, cp1y, x, y)` quadratic bezier curve from current pen position to end point specified
- `bezierCurveTo(cp1x, cp1y, cp2x, cp2y, x, y)` draws curve from current pen position to end point specified
- `rect(x, y, width, height)` draws rectangle, top left corner specified

### Path2D objects
- `Path2d()` constructor returns newly instantiated Path2d Object

# Colors
- **fillstyle** = color for filling
- **strokeStyle** = color for outlines
- **globalAlpha** = transparencyValue to all future shapes

### Line Styles
- **lineWidth = value**
- **lineCap = type**
- **lineJoin = type**
- **miterLimit = value**
- **`getLineDash()`**
- **`setLineDash(segments)`**
- **`lineDashOffset = value`**
- **`createLinearGradient(x1, y1, x2, y2)`88
- **`createRadialGradient(x1, y1, r1, c2, y2, r2)`**
- **`createPattern(image, type)`**
  - repeat
  - repeat -x
  - repeate -y
  - np-repeat
- **shadowOffsetX = float** 
- **shadowOffsetY = float**
- **shadowBlur = float**
- **shadowColor = color**

### Drawing Text
- **`fillText(text, x, y, [, maxWidth])`**
- **`strokeText(text, x, y [, maxWidth])`**
- **font = value**
- **textAlign = value**
- **textBaseline = value**
- **direction = value**
- **`measureText()`**


[Home](../README.md)