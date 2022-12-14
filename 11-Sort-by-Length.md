# Sort by Length

## Problem

Given an array of strings, sort them in the order of increasing lengths. If two strings have the same length, their relative order must be the same as in the initial array.

Example:

`inputArray = ["abc", "", "aaa", "a", "zz"]`

output should be:

`sortByLength(inputArray) = ["", "a", "zz", "abc", "aaa"]`

## Solution

```
const sortByLength = (strs, ascending) => {
    return ascending 
    ? strs.sort((a,b) => a.length - b.length) 
    : strs.sort((a,b) => b.length - a.length)
}

const strs = ["abc", "", "aaa", "a", "zz"];

console.log(sortByLength(strs, true));
// ["", "a", "zz", "abc", "aaa"]
```

