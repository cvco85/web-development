## Variables

Variables in programming are similar to variables in maths. 

However, if variables are used in maths to express something we don't know, in programming that never happens, we always know what's the value of a variable.

In programming, variables are explicitly defined, and being more technical, *a variable is a named location in memory where data can be stored*. There are some languages who require variables to have defined types, **strong typed languages** and there are others who are not that strict, called **weak typed languages**.

The process of *giving a name* to a memory address is called **creating, allocating or declaring** a variable. There are languages which automatically initialize variables and others you have to clearly do that *manually*.

```
area = pi * r * r
```

The declaration above is similar to a math notation, however, what it does is telling the computer to get values from different memory addresses and multiply them.
The normal flow how be to the computer to get the value stored in the *p* memory address as well as the value that's in the *r* address, after that it multiplies and saves the result in *area* memory address.

Example of some operators
```
X = 8 // X is now 8
X += 1 // X is now 9
X –= 3 // X is now 6
X /= 2 // X is now 3
X *= 4 // X is now 12
```

## Variable types

### Integer

Integer values and variables are exact representations of the mathematical integers. The range of number that can be stored is finite and determined by the size of the *memory location* used. 

Example of a language that requires developer to specify variable types.

```c
int numberOfDays = 30;
```

### Boolean

Boolean variables use a single bit in memory and that's why it can only store two values (1 or 0, true or false). An example of a use of a Boolean variable is something like "Customer wanted cheese on his burger?".

#### Relational Operators

Compares two or more values and returns a boolean response. 

**greater than (>)**
**greather than or equal (>=)**
**less than (<)**
**less than or equal (<=)**
**equal (==)**
**not equal (!=)**

#### Logical Operators

Logical operators are used to make decisions recurring to variable values, also returning a boolean.

**and** - only evaluates to true when both values are true.

**or** - evaluates to true when one of the values is true.

```
// AND
(1+2) > 0 AND (1-3) > 4 # false

(1+2) > 0 AND (1+3) == 4 # true

// OR
(1+2) > 0 OR (1-3) > 4 # true

(1+2) < 0 AND (1+3) <= 4 # false
```

### String

A string is a sequence of characters, it can be understood as a data type but in its genesis it is an array of bytes that stores a sequence of elements.

```javascript
var name = "FLAG Lisboa";
var course = "Introduction to web development";
```

### Array

An array is a data structure consisting in a collection of elements (either values of variables), identified by at least one index or key. The simples data structure is a linear array, also called one-dimensional array. Array indexes start on 0.

```javascript
var shoppingCart = [
  "Ball",
  "Bread",
  "Milk"
];

shoppingCart[0] // Ball
shoppingCart[2] // Milk
```
