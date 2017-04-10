# Functions

One of the biggest principles of programming is that we should destruct our problems into **smaller problems**.

This way, it is easier to the developer to reason about the problem, to make very simple code and to be able to reuse that code later.

To accomplish that, programming languages have functions, or subroutines.

A function is no more than a piece of code than can be *called* from other part of the code.

The function below says "Hello" 10 times.

```javascript
function sayHello() {
  var numberOfTimes = 10;
  var numberOfTimesSaid = 0;

  while (numberOfTimesSaid < numberOfTimes) {
    console.log('Hello');
    numberOfTimesSaid += 1;
  }
}

sayHello();
```
