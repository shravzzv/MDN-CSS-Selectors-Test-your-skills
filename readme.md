# [Test Your Skills - Selectors](https://developer.mozilla.org/en-US/docs/Learn/CSS/Building_blocks/Selectors/Selectors_Tasks)

From the MDN Web Docs

## Task 1

In this task, use CSS to do the following things, without changing the HTML:

- Make `<h1>` headings blue.
- Give `<h2>` headings a blue background and white text.
- Cause text wrapped in a `<span>` to have a font-size of 200%.

Your final result should look like the image below:

![task 1](https://developer.mozilla.org/en-US/docs/Learn/CSS/Building_blocks/Selectors/Selectors_Tasks/selectors1.jpg)

### Solution for Task 1

```css
h1 {
  color: blue;
}
h2 {
  background-color: blue;
  color: white;
}
span {
  font-size: 200%;
}
```

## Task 2

In this task, we want you to make the following changes to the look of the content in this example, without changing the HTML:

- Give the element with an `id` of `special` a yellow background.
- Give the element with a `class` of `alert` a 1px grey border.
- If the element with a `class` of `alert` also has a class of `stop`, make the background red.
- If the element with a `class` of `alert` also has a class of `go`, make the background green.

Your final result should look like the image below:

![task 2](https://developer.mozilla.org/en-US/docs/Learn/CSS/Building_blocks/Selectors/Selectors_Tasks/selectors2.jpg)

### Solution for Task 2

```css
#special {
  background-color: yellow;
}
.alert {
  border: 1px solid grey;
}
.alert.stop {
  background-color: red;
}
.alert.go {
  background-color: green;
}
```

## Task 3

In this task, we want you to make the following changes without adding to the HTML:

- Style links, making the link-state orange, visited links green, and remove the underline on hover.
- Make the first element inside the container `font-size: 150%` and the first line of that element `red`.
- Stripe every other row in the table by selecting these rows and giving them a `background-color` of `#333` and foreground of `white`.

Your final result should look like the image below:

![task 3](https://developer.mozilla.org/en-US/docs/Learn/CSS/Building_blocks/Selectors/Selectors_Tasks/selectors3.jpg)

### Solution for Task 3

```css
a:link {
  color: orange;
}
a:visited {
  color: green;
}
a:hover {
  text-decoration: none;
}

.container > :first-child {
  font-size: 150%;
}
.container > :first-child::first-line {
  color: red;
}

table tr:nth-of-type(even) {
  background-color: #333;
  color: white;
}
```

## Task 4

In this task, we want you to do the following:

- Make any paragraph that directly follows an `<h2>` element red.
- Remove the bullets and add a `1px grey bottom border` only to list items that are a direct child of the `ul` with a class of `list`.

Your final result should look like the image below:

![task 4](https://developer.mozilla.org/en-US/docs/Learn/CSS/Building_blocks/Selectors/Selectors_Tasks/selectors4.jpg)

### Solution for Task 4

```css
h2 + p {
  color: red;
}

ul.list > li {
  list-style-type: none;
  border-bottom: 1px solid grey;
}
```

## Task 5

In this task, add CSS using `attribute` selectors to do the following:

- Target the `<a>` element with a `title` attribute and make the `border-color: pink`.
- Target the `<a>` element with an `href` attribute that contains the word `contact` somewhere in its value and make the `border-color: orange`.
- Target the `<a>` element with an href value starting with `https` and give it a `border-color: green`.

Your final result should look like the image below:

![task 5](https://developer.mozilla.org/en-US/docs/Learn/CSS/Building_blocks/Selectors/Selectors_Tasks/selectors-attribute.png)

### Solution for Task 5

```css
a[title] {
  border-color: pink;
}

a[href*='contact'] {
  border-color: orange;
}

a[href^='https'] {
  border-color: green;
}
```

<style>
  img[alt]{
    max-width: 500px;
    margin-left: 0;
    display: block;
    box-shadow: rgba(60, 64, 67, 0.3) 0px 1px 2px 0px, rgba(60, 64, 67, 0.15) 0px 2px 6px 2px;
    border-radius: 10px;
  }
</style>
