# Forms
- **Form Controls** 
  - adding text
  - making choices
  - submitting forms
- **Form Structures** 
  - `<form>` form controls live here
    - action attribute
    - method
      - get
      - post
    - `<input>`
      - type="text
        - name
        - maxlength
      - type="password"
        - name
        - size
        - maxlength
      - type="radio"
        - name
        - value
        - checked
      - type="checkbox"
        - name
        - value
        - checked
      - type="file"
      - type="submit"
        - name
        - value
      - type="image"
      - type="hidden"
      - type="date"
      - type="email"
      - type="url"
      - type="search"
      - placeholder attribute with value shown in text box
  - `<textarea>` multi line text input
  - `<select>` drop down list box
    - name
  - `<option>` specify options to select from
    - value
    - selected
    - size
    - multiple
  - `<button>` creates a button
  - `<label>` 
    - for
  - `<fieldset>` group related form controls inside
  - `<legend>` after opening fieldset, contains caption
  - **form validation** messages if not filled correctly

# Lists, Tables & Forms
- `list-style-type:` control shape or style of bullet point
- `list-style-image:` image acts like bullet point
- `list-style-position:`  indents list
- `list-style:` shorthand for list styles
- **Styling Forms** make forms more attractive
- **Align Form Controls** form controls may not align 
- **cursor styles** different style to pointer

# Events
- interactions create events
- events trigger code
- code responds to users
- when events occur they are **fired** or **raised**
- events trigger a function or script
- **event handling**
  - select the element node for script to respond to
  - indiciated event on selected node to trigger response
  - state code to run when event occurs
- bind event to element
  - **HTML event handlers** bad practice, seperate html and js
  - **traditional dom** can only use one function
    - `element.onevent = functionName;`
  - **dom level 2 event listeners** favored way, trigger multiple
  `element.addEventListener('event', functionName [, Boolean]);`
  - **event flow** html elements nest inside other elements
  - **event object** tells info about event and element it happened on
  - **event delegations** to many listeners slow down a page
  - **event types**
    - **user interface** interact in browser window
    - **load** fires when web page has finished loading
    - **focus & blur** gain or lose focus on html when interacted with
    - **mouse** fired when mouse is moved/buttons clicked
    - **Events Occur**
      - screen
      - page
      - client
    - **keyboard** fired when keyboard interacted
    - **form events** 
      - submit
      - change
      - input
    - **mutation events and observors** elements added or removed from the dom triggers mutation






[Home](../README.md)