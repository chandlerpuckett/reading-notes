# Lists / Boxes / Decisions & Loops

## Cheatsheet

### Lists:
`<ol>` : ordered list
`<li>` : list item placed between tags
`<ul>` : unordered list
`<dl>` : definition list
`<dt>` : definition term
`<dd>` : used to contain definition

### CSS - BOXES:
box dimensions (width, height)
- min-width, max-width
limiting height: 
- min-height, max-height

overflow: (hidden, or scroll)

border, margin, padding
border-width: (px, or thin/medium/thick)
  - individual sides controlled with top, bottom, left, right

border-style: (solid, dotted, dashed, double, groove, ridge, inset, outset)
border-color
shorthand:
  - border: width, style, color;

margin: gap between boxes

in order to center content, or inside an element, set left & right margin to auto
must define width of box

IE6 Box Model

display: (inline, block, inline-block, none)
visibility: hidden;

border-image
box-shadow (horizontal offset, vertical offest, blur distance, spread of shadow)

border-radius

### Decision / Loops

# Logic & Loops
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