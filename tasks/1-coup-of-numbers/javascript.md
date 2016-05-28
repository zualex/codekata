# Coup of numbers - decision on javascript

### [return to task](README.md)

```javascript
const reverseInt = (num) => {
    const str = String(Math.abs(num));
    let reversedStr = '';

    let i = str.length - 1;
    while (i >= 0) {
        reversedStr += str[i];
        i--;
    }

    const reverseInt = Number(reversedStr);

    return num >= 0 ? reverseInt : -reverseInt;
}
```
