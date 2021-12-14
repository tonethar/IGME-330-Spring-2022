## I. Course Topics

1. Add ES6 Modules to Technobabble
1. Ajax/XHR Review to add JSON to Technobabble
1. Bulma
1. Web Components
1. More Ajax - Fetch/Promises
1. P1 Prototype (& localStorage review)
1. Mapbox
1. Firebase
1. P1 Final
1. Canvas
1. Creative coding - Lorenz, Phyllotaxis, Open Simplex Noise, Life, Walkers
1. Audio Visualization
1. Game (optional) Cage Clicker
1. ML with ml5 & Teachable machine
1. Better JS concepts coverage

- We covered these all this semester and it mostly fit. I think with more efficient assignments/HW of Ajax & Web Components we can cover it all BETTER

<hr>

## II. Demos (additional topics)

- PHP Proxy Server/Web Api "Wrapper"
- Interactive Adventure App - "componentize" it over time
- Parallax?
  - https://dev.to/ibrahima92/make-a-parallax-effect-with-10-lines-of-javascript-3hia
  - https://www.youtube.com/watch?v=00xjZxL8ypM

<hr>

## III. HWs
- Star Wars App
- Statistics App
- Blackout Poetry Maker
- Falling Sand? (canvas)

<hr>

## IV. JS Topics
1. `const`, `let`, `function`, arrow functions
2. Passing arguments in event handlers
    - inline anonymous function wrapper
    - `e.target` and params passed as attributes
    - `this` and params passed as attributes
3. `this` binding issue seen in Web Component event handlers - fix with:
    - inline anonymous function wrapper
    - `function.bind()` in constructor
    - arrow functions as methods
4. IIFE
5. object and array destructuring
    - destructuring in function assignments
7. method chaining
8. array methods - `forEach()`, `map()`, `reduce()`, `join()`
9. HTML string production: method chaining, template strings, `array.map()`. `array.join()`
10. "inline logical operators" - ternary operator, short circuiting, null coalescing, optional chaining
11. ES6 Classes & Objects
    - `Object.seal()` in constructor
    - prototypical inheritance
12. transpiling - Node & rollup.js?
13. module types - https://dev.to/iggredible/what-the-heck-are-cjs-amd-umd-and-esm-ikm

<hr>

## V. Other Topics
1. `localStorage` - covered in 235 - but I wonder if we need a demo covering how to put all the site data under a single object?
1. Mapbox
2. Firebase
    - https://stackoverflow.com/questions/31423124/how-to-increment-a-record-in-firebase/69650067#69650067
3. Passing data via `location.hash` or `location.search` - https://stackoverflow.com/questions/13509089/passing-data-from-one-web-page-to-another/66557503#66557503
4. Routing? (prob. no time)

<hr>

## V. Links and Inspirations
- https://mkremins.github.io/
- http://michaelkrzyzaniak.com
- https://bengrosser.com

<hr>

## VI. Code Snippets

1) Destructuring with function arg assignment

```js
function makeSprite ({x=0, y=0, width=10, height=10, imageUrl} = {}) {
	console.log(x, y, width, height, imageUrl);
}

// logs 100,200,10,10,undefined
makeSprite({
	x: 100,
	y: 200,
});
```

2) `async` IIFE

```js
(async () => {
	await someAsyncFunction();
})();
```

- https://usefulangle.com/post/248/javascript-async-anonymous-function-iife

<hr>

## VII. Project Notes

- For Project 3, make "Good starting state" a requirement with a deduction if it's not properly done


