# JavaScript Destructuring and ES2015 Refactoring Exercises

This repository contains a set of JavaScript exercises focusing on object and array destructuring, as well as refactoring ES5 code into ES2015.

## Exercises

### Destructuring Exercise

#### Object Destructuring 1
What does the following code return/print?
```javascript
let facts = { numPlanets: 8, yearNeptuneDiscovered: 1846 };
let { numPlanets, yearNeptuneDiscovered } = facts;

console.log(numPlanets); // ?
console.log(yearNeptuneDiscovered); // ?
```

#### Object Destructuring 2
What does the following code return/print?
```javascript
let planetFacts = {
  numPlanets: 8,
  yearNeptuneDiscovered: 1846,
  yearMarsDiscovered: 1659
};

let { numPlanets, ...discoveryYears } = planetFacts;

console.log(discoveryYears); // ?
```

#### Object Destructuring 3
What does the following code return/print?
```javascript
function getUserData({ firstName, favoriteColor = "green" }){
  return `Your name is ${firstName} and you like ${favoriteColor}`;
}

getUserData({ firstName: "Alejandro", favoriteColor: "purple" }) // ?
getUserData({ firstName: "Melissa" }) // ?
getUserData({}) // ?
```

#### Array Destructuring 1
What does the following code return/print?
```javascript
let [first, second, third] = ["Maya", "Marisa", "Chi"];

console.log(first); // ?
console.log(second); // ?
console.log(third); // ?
```

#### Array Destructuring 2
What does the following code return/print?
```javascript
let [raindrops, whiskers, ...aFewOfMyFavoriteThings] = [
  "Raindrops on roses",
  "whiskers on kittens",
  "Bright copper kettles",
  "warm woolen mittens",
  "Brown paper packages tied up with strings"
];

console.log(raindrops); // ?
console.log(whiskers); // ?
console.log(aFewOfMyFavoriteThings); // ?
```

#### Array Destructuring 3
What does the following code return/print?
```javascript
let numbers = [10, 20, 30];
[numbers[1], numbers[2]] = [numbers[2], numbers[1]];

console.log(numbers); // ?
```

### ES2015 Refactoring

#### ES5 Assigning Variables to Object Properties
Refactor the following ES5 code to use ES2015 object destructuring.
```javascript
var obj = {
  numbers: {
    a: 1,
    b: 2
  }
};

var a = obj.numbers.a;
var b = obj.numbers.b;
```

#### ES2015 Object Destructuring
Refactor the above code to use ES2015 object destructuring.

#### ES5 Array Swap
Refactor the following ES5 code to use ES2015 array destructuring for swapping values.
```javascript
var arr = [1, 2];
var temp = arr[0];
arr[0] = arr[1];
arr[1] = temp;
```

#### ES2015 One-Line Array Swap with Destructuring
Refactor the above code to use ES2015 one-line array swap with destructuring.

#### raceResults()
Write a function called `raceResults` which accepts a single array argument. It should return an object with the keys `first`, `second`, `third`, and `rest`.

- `first`: the first element in the array
- `second`: the second element in the array
- `third`: the third element in the array
- `rest`: all other elements in the array

Write a one-line function to make this work using:
- An arrow function
- Destructuring
- Enhanced object assignment (same key/value shortcut)

```javascript
raceResults(['Tom', 'Margaret', 'Allison', 'David', 'Pierre']);

/*
  {
    first: "Tom",
    second: "Margaret",
    third: "Allison",
    rest: ["David", "Pierre"]
  }
*/
```

### Notes
Please do not include the solutions in the code files. The purpose of these exercises is to practice and understand the concepts.

