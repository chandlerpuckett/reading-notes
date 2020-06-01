# Introductory HTML & Javascript

## HTML

- HTML is the structure & content of a webpage
- headings & subheadings create a heirarchy of information
> **tags act like containers**

the `<body>` tag contains all content shown on the main browser window
the `<head>` tag contains information *about* the page
    > the `<title>` element is usually found inside the head, the content here will be shown in the top of the browser, above the URL, or on the tab

***View Source is a helpful tool to view the code of an existing webpage***

## EXTRA MARKUP

- *id* & *class* attributes allow you to identify particular elements
- group elements together on your page using `<div>` or `<span>`
    > (it's more appropriate to use `<section>` rather than `<div>` tags)
- in order to use special characters reserved for HTML code on your page you must use an **escape character**

## HTML 5 LAYOUT

- HTML 5 introduces a new set of elements that allow you to divide up the parts of a page
    - these names include the content contained inside the element
- these new elements were introduced so authors & developers could better describe the structure of the page & to assist newer accessibility technologies such as screen readers to ignore parts such headers & footers & get straight to the content
    - search engines also might place more weight on the content in an `<article>` element than that in the `<header>` or `<footer>`

ELEMENTS: header/footer, nav, articles, aside, section, hgroup, figure, figcaption, div
> `<a>` can be placed around a block level element that turns an entire block into a link

## PROCESS & DESIGN

- decide & understand who your target audience is, & design your website accordingly
    - individuals? companies?
- Why is someone visiting your website?
    - understand their motivations & specific goals
    - what is your visitor trying to achieve?

Create a ***SITE MAP***
    - plan & organize your layout
    - focus on the goals you want your visitor to achieve

Create a ***WIREFRAME***
    - this is a simple sketch of key information that needs to go on each page of a site. it shows the hierarchy of the information and space required

> Use the concept of **visual hierarchy** to help user focus on the key message & to draw attention & guide user to subsequent messages

- Be **concise**, **clear**, and **selective** with your navigation styling

- Design is about *communication*

## JAVASCRIPT INTRO

#### What is a script & how do I create one?
- A script is a series of instructions that a computer follows in order to achieve a goal

> State your goal first, then list the tasks that need to be completed in order to solve it
1. Define the goal
2. Design the script
    - make a flowchart!
    - breakdown & list the individual steps needed 
3. Code each step!


#### How do computers fit in with the world around them?
- Computers create models of the world using data

**Objects**`(things)` 
- each object can have its own:
    - properties
    - events
    - methods
**Properties**`(characteristics)`
- specific values determining the characteristics of an object

What is an ***Event***?
- user interaction with objects on a web page

> Scripts often use different events to trigger different types of functionality

**Methods**
- represent how people interact with an object in the real world
- changes the value of one or more of that object's properties
- a method contains instructions that together represent one task

#### How do I write a script for a web page?

HTML - Content
CSS - Presentation Layer
Javascript - Behavior Layer

These three layers form the basis of a popular approach to building web pages called *progressive enhancement*

- scripts are most often found before the closing `</body>` tag
- alternatively, scripts are ran wherever they may be found in the HTML










[home](https://chandlerpuckett.github.io/reading-notes)

