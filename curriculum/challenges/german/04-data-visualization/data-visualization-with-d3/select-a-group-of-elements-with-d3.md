---
id: 587d7fa6367417b2b2512bc3
title: Select a Group of Elements with D3
challengeType: 6
forumTopicId: 301490
dashedName: select-a-group-of-elements-with-d3
---

# --description--

D3 also has the `selectAll()` method to select a group of elements. It returns an array of HTML nodes for all the items in the document that match the input string. Hier ist ein Beispiel, um alle Anker-Tags in einem Dokument auszuwählen:

```js
const anchors = d3.selectAll("a");
```

Like the `select()` method, `selectAll()` supports method chaining, and you can use it with other methods.

# --instructions--

Select all of the `li` tags in the document, and change their text to the string `list item` by chaining the `.text()` method.

# --hints--

There should be 3 `li` elements on the page, and the text in each one should say `list item`. Die Groß- und Kleinschreibung und die Abstände sollten genau übereinstimmen.

```js
assert(
  $('li')
    .text()
    .match(/list item/g).length == 3
);
```

Your code should access the `d3` object.

```js
assert(code.match(/d3/g));
```

Your code should use the `selectAll` method.

```js
assert(code.match(/\.selectAll/g));
```

# --seed--

## --seed-contents--

```html
<body>
  <ul>
    <li>Example</li>
    <li>Example</li>
    <li>Example</li>
  </ul>
  <script>
    // Add your code below this line



    // Add your code above this line
  </script>
</body>
```

# --solutions--

```html
<body>
  <ul>
    <li>Example</li>
    <li>Example</li>
    <li>Example</li>
  </ul>
  <script>
    d3.selectAll("li")
      .text("list item")
  </script>
</body>
```
