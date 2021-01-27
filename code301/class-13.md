# Sending Form Data

## Client/server architecture
  - client sends request to server
  - server answers the request

HTML form is a convenient way to send data to a server.
  
  - action
    - defines where data gets sent
    - value = valid relative or absolute url

    ```<form action="">```

-  method
  - defines how data is sent
  - two methods GET and POST
  - GET
      - asks server to send back resource
  - POST
      - browser talks to server
      - asks for response
      - takes in data provided and uses it in response
  
- Viewing HTTP requests
  - never displayed to user
  - use GET when data is not sensitive
  - use POST when it is sensitive
  - use POST for larger files

- Retrieving data
  - server receives a string
  - string is parsed
  - data is retrived as a list of key/value pairs
  - can be accessed with different platforms and frameworks.
     - PHP
    - Python
     - Django
    - Express
  
- Special requirements when sending files
  - files are binary data
  - other data is text data
  - HTTP is generally for text
    - method = POST
    - enctype = multipart/form-data
      
   ```   - input type="file" ```

- Security Issues
  - HTML forms most common place to attack server
  - sanitize all daya that comes back to server
  - escape dangerous characters
  - limit incoming data
  - sandbox uploaded files

[Home](../README.md)