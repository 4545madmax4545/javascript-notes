# JavaScript Truthy & Falsy

## What are Truthy and Falsy?

When JavaScript evaluates a condition:

```js
if (something) {
  // run this
}
```

JavaScript converts the value into a boolean.

This automatic conversion is called **Boolean Coercion**.

---

## Falsy Values (Only 8)

These values become `false` in a boolean context.

### 1. false

```js
if (false) {
  console.log("Hello");
}
```

Output:

```
Doesn't run
```

---

### 2. 0

```js
if (0) {
  console.log("Hello");
}
```

Output:

```
Doesn't run
```

---

### 3. -0

```js
if (-0) {
  console.log("Hello");
}
```

Output:

```
Doesn't run
```

---

### 4. 0n (BigInt Zero)

```js
if (0n) {
  console.log("Hello");
}
```

Output:

```
Doesn't run
```

---

### 5. ""

```js
if ("") {
  console.log("Hello");
}
```

Output:

```
Doesn't run
```

---

### 6. null

```js
if (null) {
  console.log("Hello");
}
```

Output:

```
Doesn't run
```

---

### 7. undefined

```js
if (undefined) {
  console.log("Hello");
}
```

Output:

```
Doesn't run
```

---

### 8. NaN

```js
if (NaN) {
  console.log("Hello");
}
```

Output:

```
Doesn't run
```

---

## Truthy Traps

### [] → Truthy

```js
if ([]) {
  console.log("Runs");
}
```

Output:

```
Runs
```

Because arrays are objects.

---

### {} → Truthy

```js
if ({}) {
  console.log("Runs");
}
```

Output:

```
Runs
```

Because objects exist.

---

### "0" → Truthy

```js
if ("0") {
  console.log("Runs");
}
```

Output:

```
Runs
```

Because it is a non-empty string.

---

### "false" → Truthy

```js
if ("false") {
  console.log("Runs");
}
```

Output:

```
Runs
```

Because it is text.

---

### -1 → Truthy

```js
if (-1) {
  console.log("Runs");
}
```

Output:

```
Runs
```

Because only 0 and -0 are falsy.

---

## Finger-Tip Revision

Only 8 Falsy Values:

* false
* 0
* -0
* 0n
* ""
* null
* undefined
* NaN

Everything Else = Truthy

---

## Truthy Traps

* [] → Truthy
* {} → Truthy
* "0" → Truthy
* "false" → Truthy
* -1 → Truthy

---

## Interview Questions

1. What are truthy and falsy values?
2. How many falsy values are there in JavaScript?
3. Name the 8 falsy values.
4. Is an empty array truthy or falsy?
5. Is an empty object truthy or falsy?
6. Is "false" truthy or falsy?
7. Is "0" truthy or falsy?

---

## Interview Answers

Truthy values become true and falsy values become false in a boolean context.

JavaScript has only 8 falsy values.

Empty arrays and empty objects are truthy because they are objects.

Non-empty strings such as "0" and "false" are truthy.

---

## Key Takeaways

✅ Memorize the 8 falsy values.

✅ Everything else is truthy.

✅ Understand truthy traps to avoid bugs.

✅ Truthy and falsy concepts are used heavily in DSA, React, and real-world applications.
