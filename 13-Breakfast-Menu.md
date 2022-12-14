# Breakfast Menu

## Problem

Breakfast Menu
- Topic: .map()
Our restaurant menu currently only shows the breakfast menu, 
as it has been hard coded into the HTML file. However, we want 
to offer a dinner menu instead. Let's fix this using .map()

## Solution

```
const dinnerFoods = ['🍝','🍔','🌮']

const setFoods = (foodList) => {
    return foodList.map(food => `<div class="food">${food}</div>`)
            .join('')
}

document.querySelector('#menu').innerHTML = setFoods(dinnerFoods)
```

