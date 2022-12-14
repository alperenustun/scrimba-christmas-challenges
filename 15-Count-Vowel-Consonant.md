# Count Vowel Consonant

## Problem

You are given a string s that consists of only lowercase English letters. If vowels ('a', 'e', 'i', 'o', 'u') are given a value of 1 and consonants are given a value of 2, return the sum of all of the letters in the input string.

Example:
- For s = "abcde", the output should be countVowelConsonants(s) = 8

## Solution

```
const consonantVowels = ["a", "e", "i", "o", "u"];

function countVowelConsonant(str) {
    const letters = str.split('');
    let total = 0;
    for(item of letters){
        total += consonantVowels.includes(item) ? 1 : 2
    }
    return total;
}
```

