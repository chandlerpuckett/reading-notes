# Text

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

##### Selectors:
  - universal selector
    -     * {}
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




[home](https://chandlerpuckett.github.io/reading-notes)