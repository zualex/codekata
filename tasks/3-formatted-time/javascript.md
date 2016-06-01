# Formatted time - decision on JavaScript

### [return to task](README.md)

```javascript
const getTime = (allMinutes) => {
  const minutesInHour = 60;

  const hour = Math.floor(allMinutes / minutesInHour);
  const minute = allMinutes % minutesInHour;

  const formattedHoures = ('0' + hour).slice(-2);
  const formattedMinutes = ('0' + minute).slice(-2);

  return formattedHoures + ':' + formattedMinutes;
}
```
