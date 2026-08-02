# Code Reusability

## Overview

Code reusability is the practice of writing code once and using it multiple times in different parts of a program.

Instead of rewriting the same logic again and again, developers create reusable components such as classes, functions, and modules.

Code reusability is one of the main goals of Object-Oriented Programming (OOP).

---

## Why It Matters

Code reusability is important because it:

- Reduces duplication
- Saves time
- Makes code easier to maintain
- Reduces bugs
- Improves productivity
- Makes applications easier to scale

Large software projects heavily depend on reusable code.

---

## Real-World Example

Imagine a company that manufactures cars.

Instead of designing a new engine for every car model, the company reuses the same engine design in multiple cars.

For example:

```text
Engine

↓

Toyota Corolla

Toyota Camry

Toyota Yaris
```

The same component is reused multiple times.

Software works in a similar way.

---

## Reusing Functions

Without code reusability:

```javascript
console.log(5 + 5);

console.log(10 + 10);

console.log(20 + 20);
```

With code reusability:

```javascript
function add(a, b) {
    return a + b;
}

console.log(add(5, 5));

console.log(add(10, 10));

console.log(add(20, 20));
```

The function can be reused whenever needed.

---

## Reusing Classes

Suppose we have a class:

```javascript
class Animal {
    eat() {
        console.log("Eating...");
    }

    sleep() {
        console.log("Sleeping...");
    }
}
```

Now multiple classes can reuse it:

```javascript
class Dog extends Animal {}

class Cat extends Animal {}

class Cow extends Animal {}
```

All classes automatically inherit:

- eat()
- sleep()

This reduces duplicate code.

---

## Visual Representation

```text
Animal

├── eat()
└── sleep()

        ↓

Dog

Cat

Cow
```

One class can be reused by many other classes.

---

## Ways to Achieve Code Reusability

### Functions

```javascript
function greet(name) {
    console.log("Hello " + name);
}
```

---

### Classes

```javascript
class Car {

}
```

---

### Inheritance

```javascript
class Dog extends Animal {

}
```

---

### Modules

```javascript
import math from "./math.js";
```

---

### Libraries

```javascript
React

Express

Lodash
```

Libraries provide reusable code written by other developers.

---

## Advantages of Code Reusability

Code reusability provides:

- Faster development
- Less code duplication
- Easier maintenance
- Better consistency
- Fewer errors
- Better teamwork

Reusable code saves both time and effort.

---

## Disadvantages of Code Reusability

Code reusability can also have some drawbacks:

- Poorly designed reusable code can become difficult to maintain.
- Too much abstraction can make code harder to understand.
- Reusing unsuitable code can create unnecessary complexity.

Good design is important.

---

## Real-World Applications

Code reusability is used in:

### Websites

Reusable buttons, forms, and navigation bars.

---

### Video Games

Reusable player, enemy, and weapon classes.

---

### Banking Systems

Reusable account and transaction systems.

---

### Mobile Apps

Reusable menus, login screens, and notifications.

---

## Common Mistakes Beginners Make

Beginners often:

- Copy and paste code repeatedly.
- Create duplicate functions.
- Ignore inheritance and modules.
- Make reusable components too complicated.

Remember:

If you are writing the same code multiple times, there is probably a better way.

---

## Key Takeaways

- Code reusability means writing code once and using it many times.
- It reduces duplication.
- Functions, classes, modules, and inheritance improve reusability.
- Reusable code is easier to maintain.
- Code reusability saves time and effort.
- Reusability is one of the main goals of OOP.

---

## Summary

Code reusability is the practice of creating code that can be used multiple times across an application. By using functions, classes, inheritance, and modules, developers can reduce duplication, improve maintainability, and build software more efficiently. Code reusability is one of the most important principles in modern software engineering.
