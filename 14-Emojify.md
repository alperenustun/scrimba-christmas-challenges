# Emojify!

## Problem

Popular services like Slack and Github allow for emoji shortscodes, meaning 
they will detect when a word in a sentence begins and ends with a colon (:)
and automatically replace that word with an emoji. 

These shortcodes allow users to add an emoji to their messages by typing a 
code rather than searching for an emoji from a list. 

For example, typing `:smile:` will replace that text with 😊 


## Solution

```
const emojis = {
    "smile": "😊",
    "angry": "😠",
    "party": "🎉",
    "heart": "💜",
    "cat":   "🐱",
    "dog":   "🐕"
}

function emojifyWord(word){
    if(word.startsWith(':') && word.endsWith(':')){
        const plainWord = word.slice(1, word.length - 1)
        return emojis[plainWord] !== undefined ? emojis[plainWord] : plainWord
    } else {
        return word
    }
}

function emojifyPhrase(phrase){
    return phrase.split(' ')
            .map(word => emojifyWord(word))
            .join(' ');
}

console.log(emojifyPhrase("I :heart: my :cat:"));       // I 💜 my 🐱
console.log(emojifyPhrase("I :heart: my :elephant:"));  // I 💜 my elephant

```
