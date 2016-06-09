# Factorial - decision on PHP

### [return to task](README.md)

```php
function factorial($n)
{
    $iter = function($n, $acc) use (&$iter)
    {
        return $n > 1 ? $iter($n - 1, $n * $acc) : $acc;
    };

    return $iter($n, 1);
}
```
