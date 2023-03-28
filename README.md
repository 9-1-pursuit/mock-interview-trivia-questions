# This is the List of All Trivia Questions and where they are being used

|                                                      Question                                                      |  Associated Lesson   |
| :----------------------------------------------------------------------------------------------------------------: | :------------------: |
|                           What is the difference between an parameter and and argument?                            |     [Control Flow](https://github.com/9-1-pursuit/unit-dsa/tree/main/control-flow)     |
|                              What is the difference between `var`, `const`, and `let`                              |     [Control Flow](https://github.com/9-1-pursuit/unit-dsa/tree/main/control-flow)       |
|                   Within a function, what is the difference between `return` and `console.log()`                   |     [Control Flow](https://github.com/9-1-pursuit/unit-dsa/tree/main/control-flow)       |
|                                               Code block, see below                                                |     [Control Flow](https://github.com/9-1-pursuit/unit-dsa/tree/main/control-flow)       |
|                                               Code block, see below                                                |     [Control Flow](https://github.com/9-1-pursuit/unit-dsa/tree/main/control-flow)       |
|                                What is the difference between `=`, `==`, and `===`                                 |         [Math](https://github.com/9-1-pursuit/unit-dsa/tree/main/math-for-devs)    |
|                                                   What is `NaN`?                                                   |         [Math](https://github.com/9-1-pursuit/unit-dsa/tree/main/math-for-devs)              |
|                                        Is `NaN == NaN` true or false, why?                                         |         [Math](https://github.com/9-1-pursuit/unit-dsa/tree/main/math-for-devs)              |
|                          Is `'McDonalds' > 'Burger King'` - true, false or an error? Why?                           |   [Strings & RegEx](https://github.com/9-1-pursuit/unit-dsa/tree/main/strings)    |
|             What are the differences between a single quote, double quote, smart quote, and backtick?              |   [Strings & RegEx](https://github.com/9-1-pursuit/unit-dsa/tree/main/strings)      |
|                              What is the difference between `a` and `'a'` in JavaScript?                               |   [Strings & RegEx](https://github.com/9-1-pursuit/unit-dsa/tree/main/strings)      |
|                  What is the difference between a function declaration and a function expression?                  |        Errors        |
|                    What is one difference between an arrow function and a function declaration?                    |        Errors        |
|                                Can a function expression be an anonymous function?                                 |        Errors        |
|                                Can a function declaration be an anonymous function?                                |        Errors        |
|                        Is an arrow function a function declaration or function expression?                         |        Errors        |
|                                What is the first index position of an array in JS?                                 |  [Arrays & Callbacks](https://github.com/pursuit-curriculum/unit-dsa/tree/main/arrays-and-callbacks)  |
|                                           What is a primitive data type?                                           |  [Arrays & Callbacks](https://github.com/pursuit-curriculum/unit-dsa/tree/main/arrays-and-callbacks)  |
|                                         Is an array a primitive data type?                                         |  [Arrays & Callbacks](https://github.com/pursuit-curriculum/unit-dsa/tree/main/arrays-and-callbacks)  |
|            What is the difference between: `for (let i = 0; i < 5; i++)` and `for (i = 0; i < 5; i++ )`            |  [Arrays & Callbacks](https://github.com/pursuit-curriculum/unit-dsa/tree/main/arrays-and-callbacks)  |
|                                          What is a higher order function?                                          | [Working with Objects](https://github.com/9-1-pursuit/unit-dsa/tree/main/objects) |
|                                            What is a callback function?                                            | [Working with Objects](https://github.com/9-1-pursuit/unit-dsa/tree/main/objects)  |
|                              What is the spread/rest `...` operator? What does it do?                              |        [Big O](https://github.com/9-1-pursuit/unit-dsa/tree/main/intro-to-big-o)         |
|                                               Code block, see below                                                |        [Big O](https://github.com/9-1-pursuit/unit-dsa/tree/main/intro-to-big-o)                |
|                                 What is the difference between `1000` and `1_000`?                                 |      [Recursion](https://github.com/9-1-pursuit/unit-dsa/tree/main/intro-to-recursion)       |
|                                             What does `parseInt()` do?                                             |      https://github.com/9-1-pursuit/unit-dsa/tree/main/intro-to-recursion       |
|                                            What does `parseFloat()` do?                                            |      https://github.com/9-1-pursuit/unit-dsa/tree/main/intro-to-recursion       |
|                                              What does `Number()` do?                                              |      https://github.com/9-1-pursuit/unit-dsa/tree/main/intro-to-recursion       |
|                                              What does `isNaN()` do?                                               |      https://github.com/9-1-pursuit/unit-dsa/tree/main/intro-to-recursion       |
| In JavaScript `?.` is the symbol for optional chaining. What is optional chaining and where/when would you use it? |         OOP          |
|                                               Code block, see below                                                |         OOP          |
|                         In JavaScript, what does the keyword static inside of a class do?                          |        OOP 2         |
|                          Why would we use the keyword static? What problem does it solve?                          |        OOP 2         |
|                                             none - pre-reading instead                                             |     Linked Lists     |
|                                             none - pre-reading instead                                             |   Stacks & Queues    |
|                                             none - pre-reading instead                                             |        Trees         |
|                                               Code block, see below                                                |  searching algos 1   |
|                                               Code block, see below                                                |  searching algos 1   |
|                                                                                                                    |  searching algos 1   |
|  if `const` declares a constant variable, why can you declare an array and still add/change and delete elements?   |  searching algos 2   |
|                                                     Code block, see blow                                           |  searching algos 2   |
|                                                                                                                    |  searching algos 2   |
|                                                                                                                    |     hash tables      |
|                                                                                                                    |     hash tables      |

## Evaluate Code Block:

### Control Flow

Do these code blocks return the same thing? What is different about them?

```js
const findFirstEvenNum = (arr) => {
  let num = 0;
  for (let i = 0; i < arr.length; i++) {
    if (arr[i] % 2 === 0) {
      num = arr[i];
      break;
    }
  }
  return num;
};
```

```js
const findFirstEvenNum = (arr) => {
  for (let i = 0; i < arr.length; i++) {
    if (arr[i] % 2 === 0) {
      return arr[i];
    }
  }
};
```

### Big O

Look at the following output

```js
const numbers = [1, 2, 3, 4, 5];
const printItems = (arr) => {
  for (let item in arr) {
    console.log(item);
  }
};

console.log(printItems(numbers));
```

The output is

```
1
2
3
4
5
undefined
```

Why is the last line `undefined`?


### OOP

1. What is wrong with the following code?

```js
const delete = (item) => {
  console.log('item was deleted')
}
```

2. What will the value be for `color`, after the following code runs, for the following instances of `Car`:
  - `newCar` 
  - `secondNewCar`

```js
class Car {
  constructor(brand, model, color = "soul red") {
    this.brand = brand;
    this.model = model;
    this.color = color;
  }
}

const newCar = new Car("Mazda", "MX-30");
const secondNewCar = new Car("Porche", "Vintage Carrera", "Yellow");
```

### Search Algos

What is the value of `newArr`

```js
const newArr = [...[1, 2, 3], ...[4, 5, 6]];
```

### Search Algos 2

What is the final value of `a` and `b`

```js
let a = 10;
let b = 20;

[a , b] = [b, a];

```

Is there any difference if the code is written like so?
```js
const a = 10;
const b = 20;

[a , b] = [b, a];

```



