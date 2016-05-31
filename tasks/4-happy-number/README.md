# Happy number

## Purpose
Implement function `happyNumber` which should return `true`, if a happy number, and `false` if not.
The number of iterations of the search process is necessary to limit the number 10.

Happy number - the result of a series of transformations of the form "the sum of the squares of numbers" will turn into one. For example:

```
7 => 72 = 49, 49 => 42 + 92 = 16 + 81 = 97, 97 => 92 + 72 = 81 + 49 = 130, 130 => 12 + 32 + 02 = 10, 10 => 12 + 02 = 1.
```

Conclusion: The original number 7 is happy.

## Example
```javascript
happyNumber(1); // true
happyNumber(7); // true
happyNumber(13); // true
happyNumber(0); // false
happyNumber(2); // false
happyNumber(90); // false
```

## Decision
- [JavaScript](javascript.md)
