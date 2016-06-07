# Formatted time - decision on JavaScript

### [return to task](README.md)

```javascript
const getTime = (allMinutes) => {
  const hour = Math.floor(allMinutes / 60);
  const minute = allMinutes % 60;

  const formattedHours = ('0' + hour).slice(-2);
  const formattedMinutes = ('0' + minute).slice(-2);

  return formattedHours + ':' + formattedMinutes;
}
```
