# Text / CSS

### Structural & Semantic Markup
> **Structural** elements are used to describe both headings and paragraphs
> **Semantic** markup provides extra information; such as where emphasis is placed in a sentence, that something you have written is a quotation (and who said it), the meaning of acronyms, and so on

**Headings**
  - 6 levels, `<h1>` through `<h6>`

use `<b>` or `<i>` for bold or italic text
wrap text in `<sup>` for superscript elements
wrap text in `<sub>` for subscript elements

  - When the browser comes across two or more spaces next to each other, it only displays one space. Similarly if it comes across a line break, it treats that as a single space too. This is known as **white space collapsing**.

use `<br />` to create line breaks
use `<hr />` for a *horizontal* rule break.
  - use this to create a break between *themes*

`<strong>` indicates that content has strong importance. words inside this tage might be said with strong emphasis. 
  - bold text

`<em>` indicates emphasis that subtly changes the meaning of a sentence. 
  - italic text

`<blockquote>` used for longer quotes that take up an entire paragraph. still used inside the paragraph tag. 
  - browsers tend to indent the contents of this element, use CSS to indent & style

`<q>` quote tag used for shorter quotes that sit within a paragraph. most folks **AVOID** using this attribute.

`<abbr>` if you use an acronym, you can use this tag to spell out the entire abbreviation

`<cite>` used for citations (rendered in italics)
`<dfn>` used for explaining new terminology (some browsers may show in italics)
`<address>` contains contact details for the author of the page (often displayed in italics)
`<ins>` underlined 
`<del>` strikethrough text
`<s>` visually displayed with strikethrough

### CSS

#### CSS is used to stylize & visually format the content on a webpage
  - allows you to create rules that control the way that each individual box (and the contents of that box) is presented.
    - uses *selectors* and *declarations*
  - you can specify several properties in one declaration, each separated by a semi-colon

link your CSS page in the `<head>` element
> `<link href="css/styles.css" type="text/css" rel="stylesheet">`

  - some authors use multiple CSS files, for example: one to control fonts & colors, another to control layout

#### Selectors:
  - universal selector
    -   `*` {}
  - type selector
    -    h1, h2, h3 
  - class selector
    -     .note {} , p.note {}
  - ID selector
    -    #introduction {}
  - child selector
    -     li>a {}
  - descendant selector
    -    p a {}
  - adjacent sibling selector
    -    h1+p {}
  - general sibling
    -   h1~p {}

***Use external style sheets!!!***

# JavaScript & Loops

### Basic JavaScript Instructions

- each individual step is known as a **statement**
  - case sensitive

// to add comments into javascript files

assign variables using var = *name*
shorthand can be used as well:

var price, quantity, total;
price = 5
quantity = 14
total = price * quantity

#### Naming Variables
1. must begin with letter, dollar sign, or underscore
2. can not use dash or a period in a variable name
3. cannot use keywords or reserved words
4. <ins>case sensitive</ins>
5. describe the information
6. if using more than one word, use capital for first letter of every word *after* the first word

- An **array** stores a list of values
  - assigned inside a pair of square brackets & each value separated by a comma
- each item inside an array is automatically assigned a number beginning with 0
- use these numbers to access or call a specific item inside the array 

> expressions rely on ***operators***

### Decision & Loops

**Evaluations** You can analyze values in your scripts to determine whether or note they match expected results

**Decisions** Using the results of evaluations, you can decide which path your script should go down

**Loops** There are also many occasions where you will want to perform the same set of steps repeatedly.

Two Components to a decision:
  1. An expression is evaluated, which returns a value
  2. A conditional statement says what to do in a given situation

### Comparison Operators
-  == : *is equal to*
- != : *is not equal to*
- === : strict equal to
- !== : strict not equal to
- `>` : greater than
- `<` : less than
- `>=` : greater than or equal to
- `<=` : less than or equal to

> ***Comparison operators*** usually return single values of true or false.
> ***Logical Operators*** allow you to compare the results of more than one comparison operator

- `&&` : **logical and**
    - this operator test more han one condition
    - if both expressions evaluate to *true* then the expression returns *true*. If just one of these returns *false* expression will return *false*
- `||` : **logical or**
    - this operator tests at least one condition
    - if either expression evaluates to *true*, then the expression returns true. if both return *false*, then the expression will return *false*
- `!` : **logical not**
    - this reverses the state of an expression.
    - if it was *false* (without the ! before it) It would return *true*. If the statement was *true*, it would return *false*

Logical expressions are evaluated left to right. If the first condition can provide enough information to get the answer, then there is no need to evaluate the second condition. 

### Loops

**For** loops: if you need to run code a specific number of times, use a *for* loop. (most common)

**While** loops: can run an infinite amount of times, code will continue to loop for as long as the condition is *true*

**Do While** loop: the do...while loop will always run the statements inside the curly braces at least once, even if the condition evaluates to false

- initialization;
- condition;
- update;




[home](https://chandlerpuckett.github.io/reading-notes)