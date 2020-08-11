# jQuery, Events, and The Dom

## CHEATSHEET

- Syntax:
  - `$ ( 'selector' ) `
  - ex: `$('li.hot)`

> jQuery has one parameter: A CSS-Style selector
example finds all of the `<li>` elements with a class of `hot`

#### jQuery Methods

OBJECT:         METHOD:
`$('li.hot).addClass('complete');`

- jQuery is cross-browser
- selecting elements is simpler and more accurate
- event handling is simpler, uses one method
- methods affect ALL the selected elements without the need to loop through each one
- after selection, you can apply multiple methods

Methods:
- .addClass()
- .hide()
- .fadeIn()
- .on()
- .remove()

##### Write Less, Do More

**BASIC SELECTORS**
- `*`
- `element`
- `#id`
- `.class`
- `selector1, selector2`

**HIERARCHY**
- ancestor descendant
- parent > child
- previous + next
- previous - siblings

**BASIC FILTERS**
- `:not(selector`
- `:first`
- `:last`
- `:even`
- `:odd`
- `:eq(index)`
- `:gt(index)`
- `:lt(index)`
- `:header`
- `:animated`
- `:focus`

#### MORE FILTERS / SELECTORS ETC PG 301 - 305

.ready() method checks that the page is ready for your code to work with - fires as soon as the DOM has loaded - can make page appear to load faster

.load(); use this when your script relies on assets to have loaded, e.g. if it needs to know the dimension of an image

**SHORTCUT FOR READY EVENT METHOD ON DOCUMENT OBJECT:**
`$(function () {
// script goes here
});`

-- creates function level scope for its variables
-- prevents naming collisions with other scripts

### UPDATING ELEMENTS

`.html()` & `.text()` both retrieve and update the content of the elements

-- `.html()` : it retrieves only the HTML inside the *first* element in the matched set, along with any of its descendants
  - to retrieve value of every element, use `.each()` 

-- `.text()` : returns content from every element in the jQuery selection, along with text from any descendants
  - to get content from `<input>` or `<textarea>` use the `.val()` method

-- `.replaceWith()` : replaces every element in a matched set with new content, also returns replaced elements


-- `.remove()` : removes all of the elements in the matched set


### INSERTING ELEMENTS

1. creating new elements in a jQuery Object
  - var $newFragment = $(`<li>`);

2. creates variable called " $newItem " and stores a jQuery object in it -- object in turn contains an `<li>` element with a class attribute and some text: 
  - var $newItem = $('`<li class="new">`item`</li>`)

### ADDING NEW ELEMENTS TO THE PAGE

-- `.before()` : method inserts content before selected elements
-- `.after()` : inserts after selected elements
-- `.prepend()` : inserts content inside the selected elements after opening tag
-- `.append()` : inserts content inside the selected elements before the closing tag

### GETTING AND SETTING ATTRIBUTE VALUES

- `.attr()` : can get *or* set a specified attribute and its value
  - $('li#one').attr('id);
  - $(li#one').attr('id','hot);

- `.removeAttr()` : removes specified attribute and its value
  - $('li#one').removeAttr('id');

- `.addClass()` : adds new value to existing value of the class; *DOES NOT OVERWRITE EXISTING VALUES*

-- `.removeClass()` : removes value from the class atrribute, leaving any other class names within the attribute intact


#### GET CSS PROPERTY
> var backgroundColor = $('li').css('background-color);

#### SET CSS PROPERTY
> $('li').css('background-color', '#272727');

*can increase or decrease values using the `+=` and `-+` operators

> $('li').css('padding-left', '+=20');

## CONTINUE ON PG 324. 
