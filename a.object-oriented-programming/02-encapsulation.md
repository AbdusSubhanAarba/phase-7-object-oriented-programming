# Encapsulation

## Overview

Encapsulation is one of the core principles of **Object-Oriented Programming (OOP)**. It is the practice of **bundling data and methods together inside a class** while restricting direct access to some of the object's internal details.

In simple terms, encapsulation protects an object's data and allows it to be accessed only through controlled methods.

Encapsulation helps keep data safe and prevents accidental modifications.

---

## Why It Matters

Encapsulation is important because it:

- Protects data from unauthorized access
- Improves security
- Makes code easier to maintain
- Prevents accidental changes
- Keeps related data and methods together

Most modern software applications use encapsulation.

---

## Real-World Example

Think of a bank account.

The account contains:

- Account number
- Balance
- Owner name

Imagine if anyone could directly change the balance:

```text
Balance = 1,000,000
```

That would be dangerous.

Instead, the bank provides methods such as:

- Deposit()
- Withdraw()
- CheckBalance()

Users interact with these methods instead of directly modifying the balance.

This is encapsulation.

---

## How Encapsulation Works

Encapsulation follows two basic rules:

1. Hide internal data.
2. Provide controlled access through methods.

Example:

```text
Bank Account

↓

Private Data

- Balance
- PIN

↓

Public Methods

- Deposit()
- Withdraw()
- CheckBalance()
```

The data is protected, while the methods provide safe access.

---

## Example in JavaScript

```javascript
class BankAccount {
    constructor(owner, balance) {
        this.owner = owner;
        this._balance = balance;
    }

    deposit(amount) {
        this._balance += amount;
    }

    withdraw(amount) {
        if (amount <= this._balance) {
            this._balance -= amount;
        }
    }

    checkBalance() {
        return this._balance;
    }
}

const account = new BankAccount("Ali", 1000);

account.deposit(500);

console.log(account.checkBalance());
```

In this example:

- `_balance` is protected data.
- `deposit()` changes the balance safely.
- `withdraw()` prevents invalid transactions.
- `checkBalance()` allows controlled access.

---

## Visual Representation

```text
Class

↓

BankAccount
```

```text
Private Data

- Balance
- PIN
```

```text
Public Methods

- Deposit()
- Withdraw()
- CheckBalance()
```

Users interact with methods instead of directly changing the data.

---

## Encapsulation in Everyday Life

### ATM Machine

You cannot directly edit your bank balance.

You must use:

- Withdraw
- Deposit
- Transfer

---

### Car

You drive the car using:

- Steering wheel
- Accelerator
- Brake

You do not directly control the engine's internal components.

---

### Mobile Phone

You interact with:

- Buttons
- Applications
- Settings

The internal hardware remains protected.

---

## Advantages of Encapsulation

Encapsulation provides:

- Better security
- Better code organization
- Easier maintenance
- More reliable programs
- Protection against accidental changes

It makes software safer and easier to manage.

---

## Disadvantages of Encapsulation

Encapsulation also has some limitations:

- Can increase code complexity
- Requires additional methods
- Takes more planning

However, its benefits usually outweigh its disadvantages.

---

## Real-World Applications

Encapsulation is used in:

- Banking systems
- Social media platforms
- E-commerce websites
- Video games
- Mobile applications

Almost every large software project uses encapsulation.

---

## Common Mistakes Beginners Make

Beginners often:

- Make all data public.
- Modify object data directly.
- Create unnecessary methods.
- Confuse encapsulation with abstraction.
- Forget to validate data before changing it.

Remember:

Data should be protected whenever possible.

---

## Key Takeaways

- Encapsulation bundles data and methods together.
- It protects an object's internal data.
- Access is controlled through methods.
- Encapsulation improves security and maintainability.
- Most real-world applications rely on encapsulation.
- Encapsulation is one of the four pillars of OOP.

---

## Summary

Encapsulation is an OOP principle that protects data by keeping it inside a class and allowing access only through controlled methods. By hiding internal details and exposing only what is necessary, encapsulation improves security, organization, and maintainability. It is widely used in real-world software systems, from banking applications to mobile apps.
