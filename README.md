# Intro to CSS

## Content

- Writing semantic HTML
- Box model
- block level elements vs inline elements
- Box sizing: border-box (non-default)
- CSS Specificity

## Tweeter Project

- [Tweeter Project](https://web.compass.lighthouselabs.ca/projects/w3-tweeter?day_number=w04d1)

## Approach

- As the weeks progress there is lesser emphasis on giving you all the resources, functions, tips that you need to complete an activity
- You're expected to research some subjects on your own
- Focus is on plain vanilla CSS for now
- CSS can be frustrating at first

## Writing semantic HTML

- Tags give meaning to the content rather than just presentation

- Give more info about the content to the browser

- Useful to search engine

- List of semantic tags introduced in HTML 5

```html
<article>
<aside>
<details>
<figcaption>
<figure>
<footer>
<header>
<main>
<mark>
<nav>
<section>
<summary>
<time>
```

## CSS Box Model

- Every HTML element has a box around it
- [Interactive box-model demo](http://guyroutledge.github.io/box-model/)
-[jsfiddle - box model](https://jsfiddle.net/dtremblay/nmLzpeo7/6/)
- Box-sizing

## Block-level, inline, and inline-block elements

### Block-Level Elements

- Block-level elements are taking 100% of the container
- Breaks the flow of the content
- `div, h1, p, li` are block-level elements

### Inline Elements

- Inline elements are taking only the space bounded by the tag
- Does not disrupt the flow of the content
- The top and bottom margins/paddings are NOT respected
- `span, em, strong` are inline elements

### Inline-block elements

- Behave like inline elements
- The top and bottom margins/paddings are respected
- Does not break the line

The CSS display property can change the type of element

```css
span {
  display: inline-block;
  color: green;
  padding: 1em;
  margin: 0.5em;
  border: 1px solid mediumblue;
}
```
- [Element Types - jsFiddle](https://jsfiddle.net/dtremblay/h8a92yvo/25/)

## Layout with Floats

- Float is a CSS positioning property.
- Initially used to wrap text around images
- Floats is used for web layouts
- Element can be floated left or right
- Since the flow is changed, elements are not part of the normal flow
- The parent element contained floated elements can collapsed

- [Floats - jsFiddle](https://jsfiddle.net/dtremblay/493tjkaz/16/)

## Flexbox

- Better way to layout elements

- [A Complete Guide to Flexbox](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)

## CSS Selector

### CSS Syntax

- selector + style block

```css

selector {
  property: value;
  property: value;
  ...
}
```

### Types of Selectors

- Basic Selector
- Class Selector
- ID Selector
- Attribute Selector
- Descendant Selector
- Adjacent Sibling

## CSS Specificity

### Add Styles

3 ways to add styles

- Inline
- Internal
- External

### Specificity Rules

- The more specific selector gets applied
- A score is attributed to a selector

  - nb ids x 100 pts
  - nb classes x 10 pts
  - nb of elements x 1pt
