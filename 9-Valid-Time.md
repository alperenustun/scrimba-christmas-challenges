# Valid Time

## Problem

Check if the given string is a correct time representation of the 24-hour clock.

Example

- For time = "13:58", the output should be `validTime(time) = true;`
- For time = "25:51", the output should be `validTime(time) = false;`
- For time = "2:76", the output should be `validTime(time) = false;`

## Solution

```
function validTime(str) {
    const minutes = str.length === 5 ? str.slice(3) : str.slice(2)
    if(parseInt(str) <= 24 && minutes <= 59){
        return true
    } else {
        return false
    }
}
```

