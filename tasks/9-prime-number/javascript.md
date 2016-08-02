# Prime number - decision on JavaScript

### [return to task](README.md)

```javascript
const isPrime = n => {
  if (n < 2) return false;

  const half = n / 2;
  for (let i = 2; i < half; i++) {
    if(n % i === 0) return false;
  }

  return true;
}
```
