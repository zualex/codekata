# Moving zeros to the end - decision on JavaScript

### [return to task](README.md)

```javascript
const moveZeros = arr =>
  arr.filter(function(x) {return x !== 0}).concat(arr.filter(function(x) {return x === 0;}));
```
