# Coup of numbers - decision on PHP

### [return to task](README.md)

```php
function reverseInt($num = 0)
{
    $numStr = (string) $num;
    $length = strlen($numStr) - 1;
    $reverseStr = '';

    for($i = $length; $i >= 0; $i--) {
        $reverseStr .=  $numStr[$i];
    }

    $reverseInt = (int) $reverseStr;


    return $num >=0 ? $reverseStr : -$reverseStr;
}
```
