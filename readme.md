# Introduction To Functions

### Objectives

By the end of this lesson, students will be able to:

- Define a function
- Differentiate between a function expression and a function declaration
- Call/Invoke different functions
- Revisit printing to the console
- Revisiting Variables

## What is a Function

### You Do (2 min)

Using our favorite developer tool, Google. Perform a quick search on `what is a function in javascript`.

### We Do

[MDN Documentation](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Functions#:~:text=A%20function%20in%20JavaScript%20is,the%20input%20and%20the%20output.):

> Functions are one of the fundamental building blocks in JavaScript. A function in JavaScript is similar to a procedure—a set of statements that performs a task or calculates a value, but for a procedure to qualify as a function, it should take some input and return an output where there is some obvious relationship between the input and the output.

Functions are small blocks of code that we use to perform repeatable actions in our program. This can range anywhere from outputting a message to performing some kind of mathematical equation.

Example:

```js
function printDog() {
  console.log('Dog')
}

function addNumber() {
  console.log(1 + 1)
}
```

Using the example functions above, if we wanted to print dog to the console several times, we would `call` or `invoke` them.

Example:

```js
function printDog() {
  console.log('Dog')
}

printDog()
printDog()
printDog()

function addNumber() {
  console.log(1 + 1)
}
```

In our console we would see `Dog` printed 3 times like this:

```sh
Dog
Dog
Dog
```

## Invoking/Calling Functions

Once a function is defined, we can use it by `invoking` or `calling` it.
Invoking a function is the action of telling the function we defined to activate or execute.

To invoke a function we take the function name and add opening and closing parentheses to it like so:

Example:

```js
// Defining a function
function printCat() {
  console.log('Cat')
}
// Invoking or Calling a function
printCat()
```

## Function Naming Conventions

Functions are named based on the action that they should perform. For example if a function should only print `dog` to the console, we would name the function `printDog`.

Function names should be short and memorable but descriptive, this will aid you and other programmers in identifying what action they are meant to perform.

Example:

A function with a long name is descriptive, but is not as easy to memorize later on:

```js
function printDogToTheConsole() {}
```

A function with a short but descriptive name is easier to memorize and easier to identify:

```js
function printDog() {}
```

## Function Declaration vs Function Expression

---

### **Function Expressions**

A function expression, is a function that we can store in a variable for later use.
When we store a function in a variable, the variable can be used as the function.

Example:

```js
const sum = function () {
  return 1 + 1
}
```

These functions are only loaded once the interpreter reaches the specific line.

### **Function Declaration**

A function declaration is loaded before any code is executed. Function declarations are `hoisted` or lifted to the top of our code.

Example:

```js
printIceCream()

function printIceCream() {
  console.log('Vanilla')
}
```

---

### We Do

Let's test some functions by using a handy tool called [Repl](https://repl.it/@anpato/Functions#index.js).

In the repl example, you will see that we **defined** a function declaration called `printCat` and a function expression stored in the variable `myName`.

The function `printCat` should print `cat` to the console.

Let's `invoke` or `call` this function by adding `printCat()` to the line below the `Invoke the Function` comment on line `5`.

Example:

```js
// Defining a function declaration
function printCat() {
  console.log('Cat')
}
// Invoking or Calling a function declaration
printCat()
```

Click on the `Run` button at the top of the page and you'll see `Cat` outputted to our console.

Now `invoke` the `myName` function as well and click on the `Run` button at the top of the page. `Sam` will be printed to the console.

## You Do (5 Min)

Open the `index.js` file and follow the instructions in the file.
Run the file to check your work.

Hint: To run javascript files in your terminal, use `node index.js`.

## Review (3 Min)

## Resources

- [What is a function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Functions#:~:text=A%20function%20in%20JavaScript%20is,the%20input%20and%20the%20output.)
- [Function Expression vs Function Declaration](https://medium.com/@mandeep1012/function-declarations-vs-function-expressions-b43646042052)
- [Invoking Functions](https://www.w3schools.com/js/js_function_invocation.asp)
