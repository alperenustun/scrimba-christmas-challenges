# Candy Sale

## Problem

It's the day after Halloween 🎃 and all the candy is on sale!
   
To buy up all the candy, put all the candy into a `shoppingCart` array. 

The new array should contain only the item and the price, like
this: 

Expected output: 
```
   [
       {item: "🍭", price: 2.99},
       {item: "🍫", price: 1.99}, 
       {item: "🍬", price: 0.89}
    ]
```

## Solution

index.js:

```
function getSaleItems(data){
    return data.filter(product => product.type === 'sweet')
            .map(product => {
                return {item: product.item, price: product.price}
            })
}
```

data.js:

```
export default [
    {
        item: "🍭",
        price: 2.99,
        type: "sweet",
    },
    {
        item: "🍫",
        price: 1.99, 
        type: "sweet",
    },
    {
        item: "🥫",
        price: 1.99, 
        type: "savory",
    },
    {
        item: "🍬",
        price: .89, 
        type: "sweet",
    },
    {
        item: "🥦",
        price: 3.99,
        type: "savory",
    }, 
    {
        item: "🍖",
        price: 3.99, 
        type: "savory",
    }, 
]
```