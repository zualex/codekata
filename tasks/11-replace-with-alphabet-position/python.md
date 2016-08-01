# Replace with alphabet position - decision on Python

### [return to task](README.md)

```python
def alphabet_position(text):
    return ' '.join(str(ord(c) - 96) for c in text.lower() if c.isalpha())
```
