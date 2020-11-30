# Class-01


## Introduction
### Web Access
- **Browsers** Chrome, Firefox, etc
- **Web Servers** special computer that hosts websites
- **Screen Readers** read contentws of a computer screen

### Websites Created
- **HTML** 
- **CSS** 
- **Javascript**

## Structure
  - **HTML** describes the structure of the page
### HTML
  - **elements** describe structure of page made up of 2 tags
    - **body** shown in main browser window
    - **head** meta data/page info not shown in window
    - **title** shown at top of browser
  - **tags**  act like containers for information 
    - opening tags
    - closing tags
    - self closing tags
  - **attributes**
    - additional info about contents of elements
    - appear in opening tag
    - made up of two parts
      - name
      - value
    
## Extra Markup
  - **DOCTYPES** declaration of HTML version *HTML5 current version* `<!DOCTYPE html>`
  - **comments** comments, not seen in window `<!-- -->`
  - **id** attribute that uniquely identifies an element  `<p id="whoAmI"></p>`
  - **class** attribute that identifies multiple elements `<p class="stayClassy"></p>`
  - **block** element that starts on a new line `<h1>, <p>, <ul>, <li>`
  - **inline** elements that continue on the same line `<a>, <b>, <em>, <img>`
  - **grouping block** group sets in a block `<div>`
  - **grouping inline** contain inline elements/text `<span>`
  - **iframes** *windowception* displays a page within your page `<iframe>` 
  - **meta** element lives in head of frame, author/content info `<meta>`
  - **escape characters** characters reserved for HTML code, have to use special codes to show on page

  ## HTML5 Layout
  - new elements to divide up a page
    - `<div>` replaced with `<header><nav><article><section>` better describes structure
  - **`<header>`** top of page, may appear in article 
  - **`<footer>`** bottom of page, may appear in article 
  - **`<article>`** stand alone or syndicated part of page
  - **`<section>`** groups related content
  - **`<aside>`** contains non-essential info about article or content container for page
  - **`<hgroup>`** groups together headings `<h1>, <h2>, etc`
  - **`<figure> and <figcaption>`** content referenced from main flow *images, videos, graphs etc*
  - **`<div>`** used when no other grouping elements apply
  - **Block level link** place `<a>` around entire block level element including children
  - **older browsers** may not know new HTML5, include CSS below
  ```  
  header, section, footer, aside, nav, article, 
  figure, figcaption {
      display: block;
  }
  ```

  ## Process and Design
  - **who**
    - **individual**
      - age
      - gender
      - location
      - education
      - occupation
      - etc
    - **Company**
      - size
      - position in company
      - budget
      - etc

  - **why** 
    - **motivations**
      - general or specific?
      - personal or professional?
      - essential or luxury
      - etc
    - **goals**
      - general info or specific?
      - repeat customer or new?
      - time senstive or not?
      - etc

  - **what** 
    - what are they trying to achieve
    - what information they need
  - **how** 
    - repeat customers or one time
    - how often supply restock or service changed
    - update?

  - **site map** diagram of pages used to structure site
    - **card sorting** organize info into groups using paper

  - **wire frames** sketch of key information that needs to go on each page, ensures all information is included on page
    - logo
    - navigation
    - headings
    - main bodies of text
    - user logins
    - etc
  - **visual design** aim to communicate
    - content
    - prioritizing
      - distinct
      - **visual hierarchy** order your eyes perceive info
        - size
        - color
        - style
        - images
    - organizing
      - grouping in blocks or chunks
      - similar style helps users associate with particular content
        - proximity
        - closure
        - white spasce
        - etc
  - **navigation** helps people find where to go
    - concise
    - clear
    - selective
    - context
    - interactive
    - consistent

  ## Javascript
   - makes pages more interactive
     - access content
     - modify content
     - program rules
     - react to events

  ### Script
  - instructions to achieve goal
    - define goal
    - design script
    - code each step
  - **vocabulary** words computer understands
  - **syntax** how words are put together
  - **programmatically** follow instructions in order
  - **flowchart** use to sketch out tasks
  - **objects** physical thing represented
  - **properties** characteristics
    - name
    - value
  - **events** how people interact with objects
  - **methods** things people need to do with objects
  - **Web Browsers** built using objects
    - **Document Object** represents html page
      - **properties** characteristics of page
      - **methods** tasks associated with document
      - **events** user clicks etc

  ### HTML, CSS, JS
  - **progressive enhancement** formed by 3 layers
    - **html** content layer, where content lives
    - **css** presentation layer, how content is presented
    - **javascript** behavior layer, change how page behaves, interactive

  - **Javascript**
    - can be put in page, not preferred
    - link seperate js file `<script src="filePath"</script>`
    - runs where it is found in the HTML


    [Home](README.md)
