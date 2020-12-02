# Class 3 

## Lists
- **ordered lists** use numbers `<ol`>
- **list** `<li>`
- **unordered list** use bullets `<ul>`
- **definition list** consists of terms and definitions`<dl>`
  - **definition term** contains term being defined`<dt>`
  - **dd** contains definition `<dd>`
- **nested lists** putting a list inside another list

## Boxes
#### Box Dimensions
Use pixels, percentages or ems to control, pixels allow accurate control, percentages or ems allow for more flexible designs.
  - **width** effect width
    - **min-width** stops content from becoming to narrow 
    - **max-width** stops text from appearing to wide
  - **height** effect height
    - **min-height** similar to min-width effecting height
    - **max-height** similiar to max-width effecting height
  ```
  p.one{
    width: px/ems/%;
    height: px/ems/%;}
  ```
  - **overflow** content bigger than box
    - **hidden** hides content
      ```
      p.one{
        overflow: hidden;}
    - **scroll** scroll through content
      ```
      p.one{
        overflow: scroll;}
      ```
  - **border** seperates edge of box for another
    - **border-width** width of border 
      - **border-top-width** indivudally change top
      - **border-right-width** change right
      - **border-bottom-width** change bottom
      - **border-left-width** change left
    - **border-style** style of border, can change individually similar to border-width
      - **solid**
      - **dotted**
      - **dashed**
      - **etc**
    - **border-color**  color of border, can change individually similar to border-width
    ```
    p {
      border-width: 5px;
      border-style: dotted;
      border-color: red;
    }
    ```
    - **shorthand** add width, style and color in shorthand
      ```
      p {
        width: 342px;
        border: 2px solid blue;}
      ```

  - **padding** space between border and content
    - **padding-top**
    - **padding-right**
    - **padding-bottom**
    - **padding-left**
    - **shorthand** clockwise starting at the top
    ```
    p {
      padding: 5px 10px 3px 6px;
    }
    ```
  - **margin** outside of border, creates space between boxes
    - **margin-top**
    - **margin-right**
    - **margin-bottom**
    - **margin-left**
    - **shorthand** same as padding
  - **whitespace** space between items on page
  - **center** set left and right margin to auto, give box width 
    - **text-align** inherited by children
  - **display**
    - **inline** block level element asks as inline
    - **block** inline acts like block
    - **inline-block** block level flow like inline while retaining block features
    - **none** hides element from page
  - **visibility** hide boxes but leave space
    - **hidden** hides element
    - **visible** shows the element
  - **border-image** appplies image to a border, slices it into 9 pieces
    - **stretch**
    - **repeat**
    - **round**
  - **box-shadow** add a drop shadow around box
    - **horizontal offset** negative value position shadow to left
    - **vertifcal offset** negative value position to top
    - **blue distance** without sh adow becomes solid line
    - **spread of shadow** expands or contracts shadow
  - **border-radius** creates rounded edges and eliptical shapes
    - **border-top-right-radius**
    - **border-bottom-right-radius**
    - **border-bottom-left-radius**
    - **border-top-left-radius**
    - **moz-border-radius**  used in some versions of browsers
    - **webkit-border-radius** used in some versions of browsers
  ## Arrays
  ```
  var colors;
  colors = ['red',
            'green',
            'custom'];
  ```
  ## Decisions and Loops
  - **if else** checks condition if false tries next condition
  - **switch statement** indicates possible value for variable, runs first correct code stops the rest
    - **switch value** variable code should run if matches value
  - **type coercion**  converts data types to complete operation
    - **weak typing** data type for value can change
    - **strong typing** specify data type
  - **Truthy and Falsy**  every value is true or false in js
    - **falsy** false
    - **truthy** true
  - **unary operator** returns a result with one operand
  - **short circuit** logical operators process left to right and stop on first result, giving that value not necesarrily a true or false
  - **loops** check condition, if true it runs
    - **for** specific number of times, loops through items in an array
    - **while** continues until true
    - **do while** always run statements in curly braces
    - **loop counters** counter used for condition
    ```
    var i;
    for (i = 0; i < 10; i++) {
    }
    ```
    - **break** terminates loop
    - **continue** stop current iteration, update and check
    - **infinite loop** code keeps running until out of memory
    


[Home](README.md)