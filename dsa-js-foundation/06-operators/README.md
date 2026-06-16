# JavaScript Operators

## What are Operators?

Operators are symbols used to perform operations on values.

Example:

```js
10 + 5
```

`+` is an operator.

---

## Arithmetic Operators

```js
10 + 5   // 15
10 - 5   // 5
10 * 5   // 50
10 / 5   // 2
10 % 3   // 1
2 ** 3   // 8
```

### DSA Usage

```js
n % 2 === 0
```

Even Number

```js
n % 2 !== 0
```

Odd Number

### Finger-Tip Memory

```text
+   Add
-   Subtract
*   Multiply
/   Divide
%   Remainder (DSA Hero)
**  Power
```

---

## Comparison Operators

```js
5 === 5   // true
5 !== 6   // true
10 > 5    // true
5 < 10    // true
10 >= 10  // true
5 <= 10   // true
```

### DSA Rule

✅ Always use `===`

❌ Avoid `==`

---

## Logical Operators

### &&

Returns the first falsy value.

```js
true && "Hello"    // "Hello"
false && "Hello"   // false
```

### ||

Returns the first truthy value.

```js
"" || "Default"      // "Default"
"Jalil" || "Guest"   // "Jalil"
```

### !

Opposite boolean value.

```js
!true    // false
!false   // true
```

### ??

Handles only null and undefined.

```js
null ?? "Guest"   // "Guest"
0 ?? "Guest"      // 0
```

### Finger-Tip Memory

```text
&& → First falsy
|| → First truthy
!  → Opposite
?? → Null/Undefined only
```

---

## Assignment Operators

```js
let sum = 0;

sum += 5;
sum -= 5;
sum *= 5;
sum /= 5;
sum %= 5;
```

### DSA Usage

```js
sum += arr[i];
```

---

## Ternary Operator

Short form of if-else.

```js
let max = a > b ? a : b;
```

### Memory Trick

```text
condition ? trueValue : falseValue
```

---

## Unary Operators

### Unary +

```js
+"5";   // 5
```

String to Number.

### !

```js
!true;   // false
```

Boolean toggle.

### typeof

```js
typeof 5;     // "number"
typeof "Hi";  // "string"
```

Checks data type.

---

## Optional Chaining

Safe property access.

```js
user?.address?.city
```

No crash.

Array example:

```js
arr?.[0]
```

### Memory Trick

```text
?. → Safe Access
```

---

## Type Checking

### typeof

```js
typeof name === "string"
```

### Array.isArray()

```js
Array.isArray([1, 2, 3])   // true
```

Use this for arrays.

---

## Skip for Now

Learn on demand.

Bitwise:

```text
& | ^ ~ << >>
```

Rare:

```text
, void >>> delete
```

Optional:

```text
||=
&&=
??=
```

---

## Interview Questions

1. What are operators?
2. What does `%` return?
3. Why should we use `===` instead of `==`?
4. What does `&&` return?
5. What does `||` return?
6. What does `??` do?
7. What is optional chaining?
8. Why use `Array.isArray()`?

---

## Key Takeaways

✅ Use `===` in DSA.

✅ `%` is heavily used in DSA.

✅ Understand `&&`, `||`, and `??`.

✅ Use `?.` for safe access.

✅ Use `Array.isArray()` for arrays.
