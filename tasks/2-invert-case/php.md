# Invert case - decision on PHP

### [return to task](README.md)

```php
function invertCase($str = '')
{
    $result = '';
    $length = mb_strlen($str);

    for ($i = 0; $i < $length; $i++) {
        $char = mb_substr($str, $i, 1);
        $isUpper = $char === mb_strtoupper($char);

        $result .= $isUpper ? mb_strtolower($char) : mb_strtoupper($char);
    }

    return $result;
}
```
