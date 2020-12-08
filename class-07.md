# Domain Modeling
process of creating a conceptual model in code for a specific problem
- **object-oriented** stores data in properties and encapsulated behaviors in methods

- **constructor function**
```
epicRating	1 to 10	Number
hasAnimals	true or false	Boolean


var EpicFailVideo = function(epicRating, hasAnimals) {
  this.epicRating = epicRating;
  this.hasAnimals = hasAnimals;
}

var parkourFail = new EpicFailVideo(7, false);
var corgiFail = new EpicFailVideo(4, true);

console.log(parkourFail);
console.log(corgiFail);
```

# Tables
Represents info in a grid format
- `<table>` creates a table
- `<tr>` start of each row
- `<td>` cell of data
- `<th>` table heading for col or row
- `colspan` attribute how many col's to run aross
- `rowspan` attribute how many row's to run across
- `thead` headings of the table sit inside here
- `tbody` body sits inside here
- `tfoot` footers insisde here
```
<table>
  <thead>
    <tr>
      <th></th>
      <th></th>
      <th></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th></th>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <th></th>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <th></th>
      <td></td>
      <td></td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td></td>
      <td></td>
      <td></td>
    </tr>
  </tfoot>
<table>
```

# Objects
- **constructor function** 
  - `var hotel = new Object();` create an object
  - ` function Hotel(name, rooms, booked) {` create multiple objects
- **dot notation** 
  - `hotel.name = Park;` update an object

- **global scope** function in top level of script
- **global variable** properies of the window object, access using the window object as well as properties
- **method of object** function defined inside of object
- **function expression** function defined as global used in method of an object refers to object it is contained in
- **arrays** are special types of objects
- **built in objects** contain functionaility common with many scripts
- **browser object model** contains objects that represent current window or tab
- **document object model** uses objects to create representation of current page
- **global javascript objects** represent things that the language needs to create a model
- **object model** group of objecs, each represent things from the real world
- **math object** properties and methods for math constants and functions ` Math.Round`
- **date object** work with dates `var today = new Date();`


[Home](README.md)
