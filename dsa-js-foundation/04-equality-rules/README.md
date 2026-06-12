# JavaScript Equality Rules

## What are Equality Rules?

Equality Rules define how JavaScript compares two values.

JavaScript provides three comparison methods:

1. `==` (Loose Equality)
2. `===` (Strict Equality)
3. `Object.is()`

---

## 1. == (Loose Equality)

`==` compares values after performing type coercion.

### Example

```js
'5' == 5
// true
```

### Why?

JavaScript converts the string to a number.

```js
5 == 5
// true
```

### Memory Trick

😊 Friendly Guard

* Adjusts
* Converts types

### DSA Rule

❌ Never use `==`

---

## 2. === (Strict Equality)

`===` compares both value and type without type conversion.

### Example

```js
'5' === 5
// false
```

### Why?

* Value: Same
* Type: Different

### Memory Trick

👮 Strict Security Officer

* No adjustment
* No conversion

### DSA Rule

✅ Always use `===`

---

## 3. Object.is()

`Object.is()` performs a more precise comparison.

### Special Case 1

```js
NaN === NaN
// false

Object.is(NaN, NaN)
// true
```

### Special Case 2

```js
0 === -0
// true

Object.is(0, -0)
// false
```

### Memory Trick

🔍 Fingerprint Scanner

* Detects tiny differences
* Handles edge cases

---

## Comparison Table

| Comparison  | Type Conversion | NaN vs NaN | 0 vs -0 |
| ----------- | --------------- | ---------- | ------- |
| ==          | Yes             | false      | true    |
| ===         | No              | false      | true    |
| Object.is() | No              | true       | false   |

---

## Finger-Tip Memory

```text
==           → Adjust 😊
===          → Strict 👮
Object.is()  → Microscope 🔍
```

---

## Interview Questions

1. What is `==`?
2. What is `===`?
3. What is `Object.is()`?
4. Why should we avoid `==` in DSA?
5. What is the difference between `===` and `Object.is()`?

---

## Interview One-Liners

**What is ==?**

It compares values after type conversion.

**What is ===?**

It compares both value and type without type conversion.

**What is Object.is()?**

It performs a precise comparison and handles `NaN` and `-0` edge cases differently.

---

## Key Takeaways

✅ Prefer `===` over `==`

✅ Use `Object.is()` only for rare edge cases

✅ Understand the reason instead of memorizing outputs
