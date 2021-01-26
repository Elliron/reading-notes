# EJS Partials

Partials make large websites easier to maintain, they are like a function, they are HTML that can be reused on different pages.  Nav bars and Footers are a common example of partials.

```
    <div class="header clearfix">
        <nav>
            <ul class="nav nav-pills pull-right">
                <li role="presentation"><a href="/">Home</a></li>
            </ul>
            <h3 class="text-muted">Node.js Blog</h3>
        </nav>
    </div>
```

  ```
        <footer class="footer">
        <p>© 90210 Lawyer Stuff.</p>
    </footer>
  ```

  ```
    <body>
        <div class="container">
            <%- include('partials/navbar') %>
            <div class="jumbotron">
                <h1>All about Node</h1>
                <p class="lead">Check out our articles below!</p>
            </div>
 
            <%- include('partials/footer') %>
        </div>
    </body>
  ```

  

[Home](../README.md)