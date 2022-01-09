# Code Style

- For your "solo" RIT coding projects, you are the only one writing the code
- But when working on a group project, there will likely be many others working on the same codebase. In these cases, a consistent code *style* can improve the readability and quality of your code. Ideally, the code uses consistent idioms so that in appears that one person wrote it
- Elements of a code style that improve of readability (but not necessarily the quality):
  - consistent indenting of code blocks (2-spaces, 4-spaces, or tabs)
  - consistent use of quotes around strings (either all single-quoted, or all double-quoted)
  - consistently 


## Code Snippet

- Try running the code below in the Chrome dev console
- It should run fine, but there are some issues, can you see any of them?

```js
const counter = 0;
const car = {
  'make':"Ford",
  "model":"Pinto",
  cylinders:4,
  "model":"Escort"
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

- Now try running the code through a *linter*:
  - https://eslint.org/demo
  - tick the "impliedStrict" checkbox
  - now tick "Enable all rules"
  - you should now see quite a few suggestions on how to improve your code!


