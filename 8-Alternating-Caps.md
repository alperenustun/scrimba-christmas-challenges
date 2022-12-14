# Alternating Caps

## Problem

Write a function that takes in a string of letters and returns a sentence in which every other letter is capitalized.

Example input: "I'm so happy it's Monday"

Example output: "I'M So hApPy iT'S MoNdAy"

## Solution

```
function altCaps(str){
    const letters = str.split('')
    return letters.map((letter,i) => i % 2 === 0 
            ? letter.toUpperCase() 
            : letter.toLowerCase())
            .join('')
}

console.log(altCaps("I'm so happy it's Monday"));
// I'M So hApPy iT'S MoNdAy
```

