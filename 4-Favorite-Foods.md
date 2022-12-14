# Favorite Foods

## Problem

- Topic: Object Destructuring
1. Edit the faveFoods object so that it contains 
your favorite foods.
2. Destructure the faveFoods object into three consts: 
breakfast, lunch, and supper.
3. Fetch the meals `<section>` from the DOM.
4. Set the innerHTML content of the meals `<section>` to a paragraph
that states what your favorite foods are for breakfast, lunch, and supper.
Use a template literal to construct the string.

## Solution

index.js:

```
const faveFoods = {
    breakfast: '🥐',
    lunch: '🍝',
    supper: '🍕'
}

const {breakfast, lunch, supper} = faveFoods;

const sentence = `For breakfast, I only like croissants ${breakfast}. For lunch, I love pasta ${lunch}, and for supper I want usually want pizza ${supper}.`;
document.querySelector('#meals').innerHTML = sentence;
```

index.html:

```
<html>
    <head>
        <link rel="stylesheet" href="index.css" />
    </head>
    <body>
        <section id="meals"></section>
        
        <script src="index.js"></script>
    </body>
</html>
```

