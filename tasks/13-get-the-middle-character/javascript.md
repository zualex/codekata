# Get the middle character - decision on JavaScript

### [return to task](README.md)

```javascript
const getMiddle = s => s.substr(Math.ceil(s.length / 2 - 1), s.length % 2 === 0 ? 2 : 1)
```
