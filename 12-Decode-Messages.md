# Decode an Alien Message

## Problem

We've received what (we assume) is a message of peace and brotherhood from 
an alien planet. They almost got it right, but the messages are 
backward. Write functions to reverse the backward messages so we can 
read what they have to say! 

## Solution

```
const title = ":htraE no od ot ffutS";
const messages = [
            "maerc eci yrT",
            "rewoT leffiE tisiV",
            "noom eht ot snamuh etacoleR",
            "egrahc ni stac tuP", 
        ]

function reverseString(str){
    return str.split('').reverse().join('');
}

function reverseStringsInArray(arr){
    return arr.map(item => reverseString(item))
}

console.log(reverseString(title));              // Stuff to do on Earth:
console.log(reverseStringsInArray(messages));   // ["Try ice cream", "Visit Eiffel Tower", "Relocate humans to the moon", "Put cats in charge"]
```

