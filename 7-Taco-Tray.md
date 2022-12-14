# Taco Tray

## Problem

- Help our chef fill a tray with tacos! 

## Solution

```
function getRandomNumberOfTacos() {
    const randomNumber = Math.floor(Math.random() * 10) + 1
    return new Array(randomNumber).fill('🌮')
}

function putTacosOnTray() {
    return getRandomNumberOfTacos().map(function (taco) {
        return `<div class="taco">${taco}</div>`
    }).join('')
}

document.getElementById('tray').innerHTML = putTacosOnTray()
```

