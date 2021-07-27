# Loop through elements, add an attribute
```js
[].forEach.call(document.querySelectorAll('input'), function(input) {
 input.setAttribute("spellcheck", "false")
});
```
