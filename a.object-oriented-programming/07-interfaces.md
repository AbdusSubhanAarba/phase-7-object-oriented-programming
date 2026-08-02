# Interfaces

## Overview

An interface is a blueprint that defines **what a class should do**, but not **how it should do it**.

It specifies a set of methods that a class must implement.

Think of an interface as a contract. If a class agrees to use an interface, it must provide all the required methods.

Interfaces help developers create consistent and organized code.

---

## Why It Matters

Interfaces are important because they:

- Define rules for classes
- Improve code organization
- Increase flexibility
- Make large projects easier to manage
- Encourage code reusability

Interfaces are widely used in large applications and team projects.

---

## Real-World Example

Imagine different payment methods:

- Credit Card
- PayPal
- Bank Transfer

All payment methods must support:

```text
pay()

refund()
```

The implementation may differ, but every payment method must provide these functions.

This is the idea behind interfaces.

---

## Interface as a Contract

An interface defines the required methods:

```text
Payment Interface

- pay()
- refund()
```

Classes that implement it:

```text
CreditCard

- pay()
- refund()
```

```text
PayPal

- pay()
- refund()
```

```text
BankTransfer

- pay()
- refund()
```

All classes follow the same contract.

---

## Example in JavaScript

JavaScript does not have traditional interfaces like Java, but we can simulate the concept.

```javascript
class CreditCard {
    pay(amount) {
        console.log(
            `Paid ${amount} using credit card`
        );
    }

    refund(amount) {
        console.log(
            `Refunded ${amount}`
        );
    }
}

class PayPal {
    pay(amount) {
        console.log(
            `Paid ${amount} using PayPal`
        );
    }

    refund(amount) {
        console.log(
            `Refunded ${amount}`
        );
    }
}
```

Both classes implement the same methods:

- `pay()`
- `refund()`

---

## Visual Representation

```text
Payment Interface

├── pay()
└── refund()

        ↓

CreditCard

├── pay()
└── refund()

        ↓

PayPal

├── pay()
└── refund()
```

Different classes follow the same rules.

---

## Another Real-World Example

Imagine vehicles.

Every vehicle should support:

```text
Vehicle Interface

- start()
- stop()
```

Classes:

```text
Car

- start()
- stop()
```

```text
Bike

- start()
- stop()
```

```text
Truck

- start()
- stop()
```

Each vehicle works differently, but all follow the same interface.

---

## Advantages of Interfaces

Interfaces provide:

- Better organization
- Better scalability
- Consistent code structure
- Easier teamwork
- More flexible applications

They become very useful in large software systems.

---

## Interfaces vs Classes

| Interface | Class |
|---|---|
| Defines rules | Contains implementation |
| Acts as a contract | Creates objects |
| Specifies what to do | Specifies how to do it |

An interface describes behavior, while a class implements that behavior.

---

## Real-World Applications

Interfaces are used in:

### Payment Systems

```text
pay()
refund()
```

---

### Database Systems

```text
connect()
disconnect()
```

---

### File Systems

```text
open()
close()
save()
```

---

### Games

```text
attack()
move()
jump()
```

Interfaces help different classes work together smoothly.

---

## Common Mistakes Beginners Make

Beginners often:

- Confuse interfaces with classes.
- Think interfaces contain implementation.
- Forget that interfaces define rules.
- Assume interfaces create objects.

Remember:

Interfaces describe **what** needs to be done, not **how** it is done.

---

## Key Takeaways

- An interface is a contract.
- Interfaces define methods that classes must implement.
- Interfaces improve code organization.
- Interfaces make software more flexible.
- Interfaces help developers work together.
- Interfaces are widely used in large applications.

---

## Summary

Interfaces are contracts that define the behavior expected from classes. They specify what methods must exist without describing how those methods should work internally. Interfaces improve code organization, flexibility, and maintainability, making them an essential concept in modern software engineering.
