# A Chain adding function (currying) - decision on JavaScript

### [return to task](README.md)

```javascript
const add = n => {
  const f = x => add(n + x);
  f.valueOf = () => n;
  return f;
}
```
