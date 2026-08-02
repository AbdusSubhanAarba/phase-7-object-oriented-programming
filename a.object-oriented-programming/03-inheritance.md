# Inheritance

## Overview

Inheritance is one of the core principles of **Object-Oriented Programming (OOP)**. It allows one class to inherit properties and methods from another class.

The class that provides the properties and methods is called the **parent class** (or superclass), while the class that inherits them is called the **child class** (or subclass).

Inheritance promotes code reuse and helps programmers build software more efficiently.

---

## Why It Matters

Inheritance is important because it:

- Reduces code duplication
- Encourages code reuse
- Makes programs easier to maintain
- Creates relationships between classes
- Simplifies large applications

Inheritance allows developers to write less code and reuse existing functionality.

---

## Real-World Example

Imagine a class called:

```text
Animal
```

Properties:

- Name
- Age

Methods:

- Eat()
- Sleep()

Now imagine another class:

```text
Dog
```

A dog is an animal, so instead of creating everything from scratch, the **Dog** class can inherit from the **Animal** class.

The Dog class automatically gets:

- Name
- Age
- Eat()
- Sleep()

and can also add its own methods:

- Bark()

---

## How Inheritance Works

Inheritance creates a parent-child relationship.

```text
Animal

↓

Dog
```

The child class inherits everything from the parent class.

Example:

```text
Parent Class

- Properties
- Methods

↓

Child Class

- Inherited Properties
- Inherited Methods
- New Properties
- New Methods
```

---

## Example in JavaScript

```javascript
class Animal {
    constructor(name) {
        this.name = name;
    }

    eat() {
        console.log("Eating...");
    }
}

class Dog extends Animal {
    bark() {
        console.log("Woof!");
    }
}

const dog = new Dog("Max");

dog.eat();

dog.bark();
```

In this example:

- `Animal` is the parent class.
- `Dog` is the child class.
- `Dog` inherits the `eat()` method.
- `Dog` adds its own `bark()` method.

---

## Visual Representation

```text
Animal

├── Name
├── Eat()
└── Sleep()

        ↓

Dog

├── Name
├── Eat()
├── Sleep()
└── Bark()
```

The child class gets everything from the parent and can add more features.

---

## Multiple Child Classes

One parent class can have multiple child classes.

```text
Vehicle

├── Car
├── Bike
└── Truck
```

All child classes inherit common properties from the parent.

---

## Advantages of Inheritance

Inheritance provides:

- Code reusability
- Better organization
- Easier maintenance
- Less duplication
- Cleaner code

It allows developers to build on top of existing classes.

---

## Disadvantages of Inheritance

Inheritance also has some limitations:

- Can make code more complex
- Deep inheritance chains can be difficult to understand
- Changes in the parent class may affect child classes

Inheritance should be used carefully.

---

## Real-World Applications

Inheritance is used in:

### Banking Systems

```text
Account

↓

Savings Account

↓

Current Account
```

---

### Video Games

```text
Character

↓

Player

↓

Enemy
```

---

### Vehicles

```text
Vehicle

↓

Car

↓

Truck
```

---

### E-commerce

```text
Product

↓

Book

↓

Electronics
```

Inheritance helps organize similar objects efficiently.

---

## Inheritance vs Composition

Inheritance means:

```text
Dog is an Animal
```

Composition means:

```text
Car has an Engine
```

Inheritance represents an **"is-a"** relationship.

Composition represents a **"has-a"** relationship.

Both are important concepts in software engineering.

---

## Common Mistakes Beginners Make

Beginners often:

- Confuse parent and child classes.
- Create unnecessary inheritance relationships.
- Think inheritance means copying code.
- Create very deep inheritance chains.
- Forget that child classes can add new functionality.

Remember:

Inheritance represents an **"is-a"** relationship.

---

## Key Takeaways

- Inheritance allows one class to inherit from another class.
- The parent class provides properties and methods.
- The child class receives those properties and methods.
- Inheritance promotes code reuse.
- It simplifies large applications.
- Inheritance is one of the four pillars of OOP.

---

## Summary

Inheritance is an OOP principle that allows classes to inherit properties and methods from other classes. By creating parent-child relationships, inheritance reduces code duplication, improves maintainability, and promotes code reuse. It is widely used in real-world applications such as banking systems, games, and e-commerce platforms, making it one of the most important concepts in software engineering.
