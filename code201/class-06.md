# Objects
- **object** group together a set of variables and functions to create a model you would recognize in the real world.  variables and functions take on new names.
  - **variables** become properties.
  - **property** tell us about an object, name of hotel, number of rooms.
  - **functions** become methods
  - **method** represent tasks associated with the object, subtracting booked rooms from total rooms.
  - **name and value** called a key, cannot have more than one key with the same name, used to access values.
  - **value** string, number, boolean, array, other object.  always a function
  ```
  var hotel = {             //Onject: hotel object
    // **properties**                    //**key**
    name: 'Quay',                        //string
    rooms: 40,                           //number
    booked 25,
    gym:true,                            //Boolean
    roomTypes:['twin'], ['double'],['']  // Array
    // **method**
    checkAvailability: function() {
      return this.rooms - this.booked;
    }
  };
  ```
  - **dot notation** access the property or method of object
    - **period** known as the member operator
    ` hotel.checkAvailability`
  
  # Document Object Model
  How browsers should create a model of HTML and how JS can access and update the contents in the browser window.
## 4 types of nodes
   - document
   - element
   - attribute
   - text

  - **DOM tree** how the browswer structures this model
  - **application programing interface API** lets humans interact with programs, lets scripts talk to each other
  
## Working with the DOM tree
- **access the elements** 
  ```
  - getElementById() id attribute
  - querySelector() returns first matching elementCSS selector
  - getElementsByClassName() selets all elements with specific value
  - getElementsByTagName() all elements with tag name
  - querySelectorA11() select all matching elements
  - parentNode selects parent of current node    - previousSibling/nextSibling selects previous or next sibling in DOM tree
  - firstchild/lastchild selects first or last child of current element
  ```
- **work with those elements**
  ```
  - Nodevalue access or update contents of text node
  - innerHTML access child elements and text content
  - textContent
  - createElement()
  - create TextNode()
  - appendChild()/removeChild()
  - className/id
  - hasAttribute()  checks
  - getAttribute()  gets value
  - setAttribute()  updates value
  - removeAttribute()  removes attribute
  ```

- **item()** return individual node from Nodelist
- **array syntaxv preferred over item()

- **repeating actions for entire nodelit**
```
var hotItems=document.querySelectorA11('li.hot');
for (var i = 0; i < hotItems.length; i++) {
  hotItems[i].className = 'cool';
}
```

- looping through a node list
```
var hotitems = document.querySelectorA11('li.hot');  //Store nodelist in array
if (hotItems.length > 0){            //if it contains items
for (var i=0; i<hotItems.length; i++) {     //loop through each item
hotItems[i].className = 'cool';     //change value of class attribute
}
}
```
- **traversing the DOM** Some browsers treat white space as a text element

- **update text node**
- **nodeValue** retrieve or amend content ` document.getElementById('one'),firstChild.nextSibling.nodeValue;`
- **document.write()** simple way to add content, rarely advised
- **element.innerHTML** get and update content
  - cross-site scripting or XSS attacks
- **DOM Manipulation** set of methods and properties that access create and update elements and text nodes




[Home](../README.md)