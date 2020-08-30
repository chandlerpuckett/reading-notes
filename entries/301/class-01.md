# Responsive Web Design

## CHEATSHEET

> Responsive and adaptive web design are closely related, and often transposed as one in the same

- **Responsive** generally means to react quickly and positively to any change

- **adaptive** means to be easily modified for a new purpose or situation

Mobile, on the other hand, generally means to build a separate website commonly on a new domain solely for mobile users
  - While this does occasionally have its place, it normally isn’t a great idea

### Responsive web design is broken down into three main components

1. **flexible layouts**
  - practice of building the layout of a website with a flexible grid
  - built with relative length units, `percentage` or `em`
  - These relative lengths are then used to declare common grid property values such as width, margin, or padding
2. **media queries**
  - it is recommend to use the `@media` rule inside of an existing style sheet to avoid any additional HTTP requests
  - There are three different logical operators available for use within media queries, including `and`, `not`, and `only`
3. **flexible media**
  - Within responsive design the most commonly used features include `min-width` and `max-width`


> Using *Minimum* & *Maximum* Prefixes
> The `min` and `max` prefixes can be used on quite a few media features. The min prefix indicates a values of greater than or equal to while the max prefix indicates a value of less than or equal to. Using min and max prefixes avoid any conflict with the general HTML syntax, specifically not using the `<` and `>` symbols.


