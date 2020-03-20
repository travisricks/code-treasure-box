# Convert Array-like things to true arrays

`Array.from` is not on the prototype, so you can't use `foo.from()`. It's a very useful method when working with DOM elements.

```javascript
const nodeList = document.querySelectorAll("ul li");

// Method 1: Convert to true Array
const nodeListArray = Array.from(nodeList);

// Method 2: Convert to true Array using the spread operator
[...nodeList];

// Now you can use map and other methods to loop
```

---

Sources:

- https://www.samanthaming.com/tidbits/1-convert-to-true-array/
- https://github.com/wesbos/es6-articles/blob/master/25%20-%20Array.from()%20and%20Array.of().md
