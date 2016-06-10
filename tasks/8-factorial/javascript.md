# Factorial - decision on JavaScript

### [return to task](README.md)

```javascript
const factorial = (n) => {
  const iter = (n, acc) => {
    return n > 1 ? iter(n - 1, n * acc) : acc;
  };

  return iter(n, 1);
}
```
