# Logic

## What is a program?

A program is a set of instructions that tell a computer how to do a task. When the computer follows those instructions, we say it executes the program.

We can make an analogy with culinary. Imagine describing the steps to do a recipe, imagine making a sandwich. 

- Get the bread
- Open it
- Get ham and cheese
- Put ham first, cheese second
- Add the top part of the bread

Those are a set of instructions to make a sandwich, programming is not that different from that.

We use to think computers are smart, but get that idea out of your mind. **Computers are dumb dumb dum**. The good part is that computers are obedient, they only make what you (or someone else) told them to do.

Yeah, that's the frustrating part, when your program is failing, is not computer's fault, no matter how your try, 99,999% of times, that's YOUR fault.

Computers are no more than machines that understand two different signals, **0** and **1**, the most basic numbering system, binary. If you want to "tell the computer directly what to do" you would have to tell them sequences of *0* and *1*. And yeah, that's almost impossible. That's why there are programming languages.

![What is a programming language?][whatIsAProgrammingLanguage]

[whatIsAProgrammingLanguage]: https://upload.wikimedia.org/wikipedia/commons/2/2d/Programming_language.png

## What is a programming language?

A programming language, is no more than a language develop to express programs. Every computer have a native programming language they understand, refered to as **machine code**. Programming languages serve as an interface between the developer and the computer.

A language is *lower level* as more closer it is to machine code, and *higher level* as it gets away from it and seems more like *human language*.

One of the lowest known languages is *assembly*. C is *higher level* than *assembly* and lower level than *python*, *java*, *javascript*, etc.

There are two types of programming languages:

- Interpreted - evaluated in real time, the computer goes line by line as the program is being executed. The program is stored in a human readable format.

- Compiled - a program goes through the program and "translates it" to *machine code*. Compiled languages are usually faster but also stricter in terms of features and types.

```assembly
// That's how you add two numbers in assembly

LUI  R1, #1
LUI  R2, #2
DADD R3, R1, R2
```

The first to lines save the number 1 and 2 into computer's memory. The last one tells the computer to add the two values and store the result. [Assembly](https://en.wikipedia.org/wiki/Assembly_language)

```c
#include <stdio.h>

int main() {
  printf("Hello World!\n");
  return 0;
}
```

```basic
10 PRINT "Hello world!"
20 END
```

```java
public class HelloWorld
{
  public static void main(string[] args)
  {
    System.out.println("Hello world!");
  }
} 
```

## How is a program organized?

A program is a list of statements. Statements are *more-or-less* and atomic piece of code, they tell the computer to *do a thing*. A lot of languages have a way of *saying the computer* that a statement is over (a lot of them use the `;`)

- Get the bread
- Open the bread

The words a language supports and "understands" are called the **language syntax**. The *syntax* changes from language to language, however, a lot of the principles are the same, those principles are called **meta programming**.

Basically, if you understand the principles and concepts, you understand how most of languages work, and that's what matters.
