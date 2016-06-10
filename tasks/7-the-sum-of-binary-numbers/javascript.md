# The sum of binary numbers - decision on JavaScript

### [return to task](README.md)

```javascript
const binarySum = (a, b) => {
  const sum = (symbolA, symblolB) => {
    let res = {
      'sum': '0',
      'save': '0'
    };

    if (symbolA + symblolB === '00') res['sum'] = '0';
    if (symbolA + symblolB === '01') res['sum'] = '1';
    if (symbolA + symblolB === '10') res['sum'] = '1';
    if (symbolA + symblolB === '11') {
      res['sum'] = '0';
      res['save'] = '1';
    }

    return res;
  }

  const reversA = a.split('').reverse().join('');
  const reversB = b.split('').reverse().join('');

  const length = a.length > b.length ? a.length : b.length;
  let reversRes = '';
  let save = '0';
  for(let i = 0; i < length; i++) {
    let symbolA = reversA[i] || '0';
    let symbolB = reversB[i] || '0';

    let sumSymbol = sum(symbolA, symbolB);
    if (save === '1') sumSymbol = sum(sumSymbol['sum'], save);

    save = sumSymbol['save'];
    reversRes += sumSymbol['sum'];
  }

  if (save === '1') reversRes += save;

  const result = reversRes.split('').reverse().join('');
  return result;
}
```
