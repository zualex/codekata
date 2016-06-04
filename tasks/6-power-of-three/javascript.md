# Power of three - decision on JavaScript

### [return to task](README.md)

```javascript
const isPowerOfThree = (num) => {
  const iter = (num, pow) => {
    if(num === 1) return true;
    if(num % pow !== 0) return false

    return iter(num / pow, pow);
  }

  return iter (num, 3);
};
```
