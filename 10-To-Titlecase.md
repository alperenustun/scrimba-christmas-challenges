# toTitleCase()

## Problem

Write a function that will capitalize every word in a sentence.  

Example Input: "everything, everywhere, all at once"

Example Output: "Everything, Everywhere, All At Once"

## Solution

```
function capitalizeWord(word){
    return `${word.slice(0,1).toUpperCase()}${word.slice(1)}`
}

function toTitleCase(str){
    return str.split(' ').map(word => capitalizeWord(word))
            .join(' ');
}

console.log(toTitleCase("pumpkin pranced purposefully across the pond"));
// Pumpkin Pranced Purposefully Across The Pond
```

