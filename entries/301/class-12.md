# EJS Partials

## CHEATSHEET

> Partials come in handy when you want to reuse the same HTML across multiple views

- think of partials as functions
- define that reusable bundle of code in a file andinclude it wherever you need it

- define as new chunks of code such as:
  - **navbar.ejs**
  - **footer.ejs**

> include in your templates is always surrounded by <% %> delimiters

**Including a partial in EJS is quite straightforward. You use <%- include( PARTIAL_FILE ) %> where the partial file is relative to the template you use it in**

- Note: The `<%- %>` tags allow us to output the **unescaped** content onto the page (notice the `-`)



