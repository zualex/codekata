# Formatted time - decision on PHP

### [return to task](README.md)

```php
function getTime($allMinutes)
{
    $hours = floor($allMinutes / 60);
    $minutes = $allMinutes % 60;

    $formattedHours = sprintf("%02d", $hours);
    $formattedMinutes = sprintf("%02d", $minutes);

    return $formattedHours . ':' . $formattedMinutes;
}
```
