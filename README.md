# Intro to CSS

## Content📣

- Approach with new material
- Writing semantic HTML
- Box model
- block level elements vs inline elements
- Box sizing: border-box (non-default)
- CSS Selector
- CSS Specificity
- Float
- Flexbox

## Approach 🆕❓

- 1️⃣ As the weeks progress there is lesser emphasis on giving you all the resources, functions, tips that you need to complete an activity
- 2️⃣ You're expected to research🔍 some subjects on your own
- 3️⃣ Focus is on plain vanilla CSS for now
- 4️⃣ CSS can be frustrating at first🙀

## New Project: Tweeter🐤

DEMO 📺

## Semantic HTML

- 🔸 Tags _give meaning_ to the content rather than just structure

- 🔸 Give more info about the content to the browser

- 🔸 Useful to search engine

- 🔸 List of semantic tags introduced in HTML 5

front-end = HTML + CSS + JavaScript

HTML = Structure of your page
CSS = styling of your page
JS = Interactivity


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

- 🔗[Semantic Tags](https://jsfiddle.net/dtremblay/cv3mk916/10/)
- 🔗[Without Semantic Tags](https://jsfiddle.net/dtremblay/v380axgz/)

## CSS Syntax

- 🔸selector + style block
- 🔸type of selectors include element, id, class

```css
selector {
  property: value;
  property: value;
  ...
}
```

### Add Styles

3 ways to add styles

- 1️⃣Inline
- 2️⃣Internal
- 3️⃣External


## CSS Box Model ⬜

- Every HTML element has a box around it 🔳
- 🔗[jsfiddle - box model](https://jsfiddle.net/dtremblay/nmLzpeo7/29/)
- 🔗[Interactive box-model demo](http://guyroutledge.github.io/box-model/)
- Box-sizing property

## Block-Level Elements

- div
- header, main, section, nav, footer
- p, ul, li

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
- [Block, inline - jsFiddle](https://jsfiddle.net/dtremblay/h8a92yvo/36/)

## CSS Layouts

- Floats
- Flexbox

## Layout with Floats🔁

- Float is a CSS positioning property
- Initially used to wrap text around images
- Floats was being used for web layouts
- Element can be floated left or right
- Since the flow is changed, elements are not part of the normal flow
- The parent element contained floated elements can collapsed

- [Floats - jsFiddle](https://jsfiddle.net/dtremblay/493tjkaz/16/)

## Flexbox 💟

- Better way to layout elements
- [Flexbox Layout Exercise](https://jsfiddle.net/dtremblay/493tjkaz/59/)
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
- Sibling Selector

- [Selectors](https://jsfiddle.net/dtremblay/e3v095ws/94/)

## CSS Specificity

### Specificity Rules

- The more specific selector gets applied
- A score is attributed to a selector

  - nb ids x 100 pts
  - nb classes x 10 pts
  - nb of elements x 1pt

* inline-style => 1000 pts


![specificity](./images/specificity1.png)
- [Selectors Specifity](https://jsfiddle.net/dtremblay/xr94uLnb/24/)
  