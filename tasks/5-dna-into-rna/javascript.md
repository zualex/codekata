# DNA into RNA - decision on JavaScript

### [return to task](README.md)

```javascript
const toRna = (dna) => {
  let rna = '';
  const length = dna.length;

  for(let i = 0; i < length; i++) {
    let symbol = '';

    if (dna[i] === 'G') symbol = 'C';
    if (dna[i] === 'C') symbol = 'G';
    if (dna[i] === 'T') symbol = 'A';
    if (dna[i] === 'A') symbol = 'U';

    rna += symbol;
  }

  return rna;
}
```
