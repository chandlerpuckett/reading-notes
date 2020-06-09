# CHEATSHEET

## Problem Domain

### Object Literals
#### JS pgs 100-105

var name = {
  name:
  rooms: 
  booked: 
  checkAvailability: function(){
    return this.rooms - this.booked;
  }
}

### DOM 
#### JS pgs 183 - 242

- DOM TREE
> model of a webpage

1. access the elements
  - individual element node
    - getElementById()
    - querySelector()
  - multiple elements (nodelists)
    - getElementsByClassName()
    - getElementsByTagName()
    - querySelectorAll()
  - traversing between element nodes
    - parentNode
    - previousSibling / nextSibling
    - firstChild / lastChild

2. work with those elements
  - access / update text nodes
    1. select the `<li>` element
    2. use the firstChild property to get the text node
    3. use the text node's only property (nodeValue) to get the text from the element
      - nodeValue *(access or update contents of a textNode)*
  - work with HTML content
    - innerHTML
    - textContent
    - createElement()
    - createTextNode()
    - appendChild() / removeChild()
  - access or update attribute values
    - hasAttribute()
    - getAttribute()
    - setAttribute()
    - removeAttribute()



[home](https://chandlerpuckett.github.io/reading-notes)
