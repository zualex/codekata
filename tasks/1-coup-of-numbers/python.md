# Coup of numbers - decision on Python

### [return to task](README.md)

```python
def reverseInt(num):
    absNum = abs(num)
    reverseNum = int(str(absNum)[::-1])
    return 	reverseNum if num > 0 else -reverseNum
```
