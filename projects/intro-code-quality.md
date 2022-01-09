# Code Quality


## Code Snippet

- Try running the code below in the Chrome dev console (omitting the `'use strict';` declaration at the top)
- It should 

```js
'use strict';
const counter = 0;
const car = {
  'make': "Ford",
  "model": "Pinto",
  cylinders: 4,
  "model": "Escort"
};

if(car.cylinders == 4){
  speed = "slow";
}else{
  speed = "not slow";
  counter++;
}

if (car.model = "Pinto") console.log("It's a Pinto");

console.log(`The ${car.model} is ${speed}`);
console.log("counter =",counter);
```
