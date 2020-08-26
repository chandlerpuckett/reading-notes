# Sending Form Data

## CHEATSHEET

### client / server architecture
- the web uses a client/server architecture that can be summarized as follows. a client (usually a web browser) sends a request to a server (most of the time a web server like Apache, Nginx, IIS, Tomcat, etc.), using the HTTP protocol
  - The server answers the request using the same protocol.

> The `<form>` element defines how the data will be sent

The two most important attributes are `action` and `method`

> The `action` attribute defines where the data gets sent. Its value must be a valid relative or absolute `URL`
  - If this attribute isn't provided, the data will be sent to the URL of the page containing the form

- The action value should be a file on the server that can handle the incoming data, including ensuring server-side validation

### C R U D 

Create, Read, Update, Delete

Method: POST, GET, PUT, DELETE
SQL: INSERT, SELECT, UPDATE, DELETE
Array: push, `arr[i]`, arr.splice, splice / pop

Can Send 3 ways:
- request.params (*differentiates route*)
- request.query (*optional things at the end*)
- request.body (*for sensitive information on the POST method*)

`id` will come from `request.params.id` 

`const{id} = request.params;`




