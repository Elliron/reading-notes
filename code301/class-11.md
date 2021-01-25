# EJS

Install

```
NPM INIT -y
npm install --save express body-parser cors ejs
```

Setup
```
var bodyParser = require('body-parser');
var path = require('path');

app.use(bodyParser());
app.set('views', path.join(_dirname, 'views'));
app.set('view engine', 'ejs');

app.get('/', function(req, res) {
  response.render('index');
});
```

Inject values into views

```
foo: 'bar'
!-- insert esj symbol and "foo" into html --!
```

For Loops and Arrays
```
people: [
  Carol
  Bob
  Tim
  Sherry
]
!-- insert into html <% for(var person of people {  <li>esj-symbol person.name esj-symbol </li>
esj-symbol } esj-symbol}) --!
```

If/Else Statement

```
<ul>
<% for(var person of people) { %>
<% if (person.name ==='Bob') { %>
  <li><% person.name %> </li>
  <% } else { %>
<li>Not <%person.name %> </li>
 <% } %>
<% } %>
</ul>
```

[Home](../README.md)