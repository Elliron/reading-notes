# Layouts
CSS treats each HTML element as if it is in a box
- **block level elements** start on new line
- **inline elements** flow in between surrounding text
- **containing elements** outter box with another box in it
- **positioning schemes**
  - **normal flow** `position:static`
  - **relative positioning**
    `position:relative`
  - **absolute positioning** `absolute:position`
- **box offset** 
  - **fixed positioning** `position:fixed`
  - **floating elements** `float`
    - clear
    - left
    - right
    - both
    - none
    - **multi-coloumn layout** 
      ```
      .coloumn {
        float: left;
        width: 500px;
        margin: 10px;
      }
      ```

  - **screen sizes** design needs to work on a range of sizes
  - **screen resolution** number of dots a screen shows
  - **page sizes** try to create pages around 960 - 1000 px wide
  - **fixed width layouts** do not change with window size
  - **liquid layouts** stretch and contract with window size
  - **layout grids** grid structure to help position items on page, how they are organized
  - **CSS frameworkds** provides code for common tasks, already written
  - **multiple style sheets** `@import` HTML element links to one style sheet, that sheet uses @import to connect to other style sheets
  - **multiple style sheets** `<link rel="stylesheet" type="text/css" href="cssLink"/>`

[Home](README.md)