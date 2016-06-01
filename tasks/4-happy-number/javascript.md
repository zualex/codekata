# Happy number - decision on JavaScript

### [return to task](README.md)

```javascript
const happyNumber = (num, callCount = 0) => {
  const sumDigits = (num) => {
    const numAsStr = String(num);
    let sum = 0;
    for (let i = 0; i < numAsStr.length; i++) {
      const digit = Number(numAsStr[i]);
      sum += digit * digit;
    }

    return sum;
  };

  const iter = (num, start, end) => {
    if(start === end){ return false; }
    if(num === 1){ return true; }

    return iter(sumDigits(num), start + 1, end);
  };

  return iter(sumDigits(num), 0, 10);
}
```
