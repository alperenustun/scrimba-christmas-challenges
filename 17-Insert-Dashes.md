# Insert Dashes

## Problem

Transform a given sentence into a new one with dashes between each two consecutive letters.

Example:

For `inputString = "aba caba"`, the output should be `insertDashes(inputString) = "a-b-a c-a-b-a"`.

## Solution

```
function insertDashes(arr) {
    return arr.split(' ')
            .map(element => [...element].join('-'))
            .join(' ')
}
```

