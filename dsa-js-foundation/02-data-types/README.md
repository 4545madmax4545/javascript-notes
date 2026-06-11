# JavaScript Data Types (Deep Dive)

## What is a Data Type?

A data type defines the kind of value stored in a variable.

Example:

```js
let name = "Jalil";
let age = 23;
```

---

# Categories of Data Types

JavaScript data types are divided into:

1. Primitive Data Types
2. Reference Data Types

---

# Primitive Data Types

Primitive values are stored directly in memory.

## String

Stores text.

```js
let name = "Jalil";
```

Real Life:
A person's name.

---

## Number

Stores numeric values.

```js
let age = 23;
```

Real Life:
Age, marks, salary.

---

## Boolean

Stores true or false.

```js
let isLoggedIn = true;
```

Real Life:
Light ON/OFF.

---

## Undefined

Variable declared but no value assigned.

```js
let city;

console.log(city);
```

Output:

```js
undefined
```

Real Life:
Empty answer sheet.

---

## Null

Intentional empty value.

```js
let user = null;
```

Real Life:
Reserved seat but nobody sitting.

---

## Symbol

Creates unique identifiers.

```js
const id = Symbol("id");
```

Real Life:
Unique Aadhaar number.

---

## BigInt

Stores very large integers.

```js
const bigNumber = 12345678901234567890n;
```

Real Life:
Population of planets 😄

---

# Reference Data Types

Stored in Heap Memory.

Variables store only memory addresses.

## Object

```js
const user = {
  name: "Jalil",
  age: 23
};
```

---

## Array

```js
const fruits = ["Apple", "Mango"];
```

---

## Function

```js
function greet() {
  console.log("Hello");
}
```

---

# Heap Memory

Reference values are stored in Heap Memory.

Example:

```js
let user = {
  name: "Jalil"
};
```

Memory:

user → Address 1001

Heap:
{name:"Jalil"}

Memory Trick:

Primitive = Cash in Pocket 💵

Reference = Locker Key 🔑

Heap = Actual Locker 🏦

---

# Important JavaScript Cases

## typeof null

```js
typeof null
```

Output:

```js
"object"
```

Reason:

Historical JavaScript bug.

Memory Trick:

null is NOT an object,
but typeof null returns "object".

---

## NaN !== NaN

```js
NaN === NaN
```

Output:

```js
false
```

Reason:

NaN is not equal to any value,
including itself.

Memory Trick:

NaN trusts nobody 😄

---

## Number.isNaN()

```js
Number.isNaN(NaN)
```

Output:

```js
true
```

Memory Trick:

NaN detector 🔍

---

## 0 === -0

```js
0 === -0
```

Output:

```js
true
```

Reason:

JavaScript normal comparison treats both as equal.

Memory Trick:

Human Eye 👀

---

## Object.is(-0, 0)

```js
Object.is(-0, 0)
```

Output:

```js
false
```

Reason:

Object.is performs stricter comparison.

Memory Trick:

Microscope 🔬

---

# Interview Questions

1. What are JavaScript Data Types?
2. Difference between Primitive and Reference Types?
3. Why does typeof null return object?
4. Why is NaN not equal to itself?
5. What is Number.isNaN()?
6. Difference between === and Object.is()?
7. What is Heap Memory?
8. What are Reference Data Types?

---

# Key Takeaways

✅ Primitive → String, Number, Boolean, Null, Undefined, Symbol, BigInt

✅ Reference → Object, Array, Function

✅ Objects are stored in Heap Memory

✅ typeof null is a historical bug

✅ NaN is not equal to itself

✅ Object.is() is stricter than ===
