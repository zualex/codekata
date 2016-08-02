# Hamming weight - decision on JavaScript

### [return to task](README.md)

```javascript
const hammingWeight = num => {
  const binaryList = num.toString(2).split('');
  return binaryList.reduce((sum, x) => sum + parseInt(x), 0);
}
```
