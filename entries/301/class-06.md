# Node, Express, API's

## CHEATSHEET

> Node.js is a javascript runtime built on Chrome's V8 JavaScript engine

### Check Version

`node -v`

- console.log will use Node's built in console module to display in a terminal window

- INSTALL A PACKAGE GLOBALLY:
  - `npm install -g 'package'`

- INSTALL A PACKAGE LOCALLY:
  - create "test" folder
  - `npm init -y`
  - `npm install 'loadash' --save`
  - create file named test.js and add:
    - `const_ = require('lodash');`

> developing apps with any modern JS framework (React or Angular) requires a working knowledge of Node and npm (maybe Yam)

- Node.js lets allows dev to run JS on the server
- Node.js is **event driven**
- uses the `libuv` library to implement asynchronous non-blocking behaviour
- blocking I/O calls should be avoided
- CPU intensive operations should be handed off to a worker thread

LOCAL SERVER:
- http:localhost:3000

`req` & `res` function arguments

- Node is suited for apps that require real-time interaction or collaboration
- building API's that handle lots of requests that are I/O driven
- performing operations on a database
- Node speaks JSON

> Express NPM

- Node can also be used as a scripting language to automate repetetive or error prone tasks


