# Invert case - decision on javascript

### [return to task](README.md)

```javascript
const invertCase = (str) => {
  let invertStr = '';
  const length = str.length;

  for (let i = 0; i < length; i++) {
    let isUpper = str[i] === str[i].toUpperCase();
    invertStr += isUpper ? str[i].toLowerCase() : str[i].toUpperCase();
  }

  return invertStr;
}
```
