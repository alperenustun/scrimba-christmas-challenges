# Panic Function

## Problem

Write a PANIC! function. The function should take in a sentence and return the same
sentence in all caps with an exclamation point (!) at the end. 

If the string is a phrase or sentence, add a 😱 emoji in between each word. 

- Example input: "Hello"
- Example output: "HELLO!"

- Example input: "I'm almost out of coffee"
- Example output: "I'M 😱 ALMOST 😱 OUT 😱 OF 😱 COFFEE!"

## Solution

```
function panic(sentence){
    return sentence.toUpperCase().split(' ').join(' 😱 ') + '!';
}
```

