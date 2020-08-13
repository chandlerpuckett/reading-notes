# CSS GRID / RegEx

## CHEATSHEET

### RegExr

> Regular expressions (regex or regexp) are extremely useful in extracting information from any text by searching for one or more matches of a specific search pattern (i.e. a specific sequence of ASCII or unicode characters).

- can be used in almost all programming languages

**Character classes**
`.`	      any character except newline
`\w\d\s`	word, digit, whitespace
`\W\D\S`	not word, digit, whitespace
`[abc]`	  any of a, b, or c
`[^abc]`	not a, b, or c
`[a-g]`	  character between a & g

**Anchors**
`^abc$`	  start / end of the string
`\b\B`	  word, not-word boundary

**Escaped characters**
`\.\*\\`	escaped special characters
`\t\n\r`	tab, linefeed, carriage return

**Groups & Lookaround**
`(abc)`	  capture group
`\1`	    backreference to group #1
`(?:abc)`	non-capturing group
`(?=abc)`	positive lookahead
`(?!abc)`	negative lookahead

**Quantifiers & Alternation**
`a*a+a?`	  0 or more, 1 or more, 0 or 1
`a{5}a{2,}`	exactly five, two or more
`a{1,3}`	  between one & three
`a+?a{2,}?`	match as few as possible
`ab|cd`	    match ab or cd

**Boundaries — \b and \B**
`\babc\b`   performs a "whole words only" search

### CSS GRID

**Parent Containers**
- display
  - grid
  - inline-grid
- grid-template-columns
- grid-template-rows
- grid-template-areas
- grid-template
  - column-gap
  - row-gap
  - grid-column-gap
  - grid-row-gap
- gap
- grid-gap
- justify-items
- align-items
- place-items
- justify-content
- align-content
- place-content
- grid-auto-columns
- grid-auto-rows
  - `<track-size>`
- grid-auto-flow
- grid

**Grid Items (Children)**
- grid-column-start
- grid-column-end
- grid-row-start
- grid-row-end
  - `<line>`
  - `span<number>`
  - `span<name>`
  - `auto`
- grid-column
- grid-row
- grid-area
- justify-self
- align-self
- place-self
