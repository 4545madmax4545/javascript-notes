# JavaScript Type Coercion

## What is Type Coercion?

Type Coercion means JavaScript automatically converts one data type into another type to perform an operation.

## Golden Rules

* `==` → Checks value only (JavaScript converts types)
* `===` → Checks value + type (No conversion)
* `+` with string → Concatenation
* `-`, `*`, `/`, `%` → Convert to Number

---

## 1. '5' + 3

### Code

```javascript
'5' + 3
```

### Output

```javascript
"53"
```

### Why?

String + Anything = String

Internally:

```javascript
'5' + '3'
```

### Real Life

```javascript
"House No: " + 5
// "House No: 5"
```

### Memory Trick

String + Anything = Join

---

## 2. '5' - 3

### Code

```javascript
'5' - 3
```

### Output

```javascript
2
```

### Why?

Math operators convert strings to numbers.

Internally:

```javascript
5 - 3
```

### Memory Trick

`-`, `*`, `/`, `%` = Number Conversion

---

## 3. '5' == 5

### Code

```javascript
'5' == 5
```

### Output

```javascript
true
```

### Why?

Loose equality checks value only.

Internally:

```javascript
5 == 5
```

### Memory Trick

`==` → Value Only

---

## 4. '5' === 5

### Code

```javascript
'5' === 5
```

### Output

```javascript
false
```

### Why?

Strict equality checks value and type.

### Memory Trick

`===` → Value + Type

---

## 5. null == undefined

### Code

```javascript
null == undefined
```

### Output

```javascript
true
```

### Why?

Special JavaScript rule.

### Memory Trick

Best Friends 🤝

---

## 6. null === undefined

### Code

```javascript
null === undefined
```

### Output

```javascript
false
```

### Why?

Different types.

### Memory Trick

Best Friends with Different ID Cards 😄

---

## 7. [] == false

### Code

```javascript
[] == false
```

### Output

```javascript
true
```

### Why?

JavaScript internally converts:

```javascript
false → 0
[] → '' → 0
0 == 0
```

### Memory Trick

JS Magic 🪄

---

## 8. [] === false

### Code

```javascript
[] === false
```

### Output

```javascript
false
```

### Why?

```javascript
[]      → Object
false   → Boolean
```

Different types.

### Memory Trick

Object ≠ Boolean

---

# Finger-Tip Revision

| Code                 | Output  | Memory Trick      |
| -------------------- | ------- | ----------------- |
| `'5' + 3`            | `"53"`  | String Joins      |
| `'5' - 3`            | `2`     | Number Conversion |
| `'5' == 5`           | `true`  | Value Only        |
| `'5' === 5`          | `false` | Value + Type      |
| `null == undefined`  | `true`  | Best Friends      |
| `null === undefined` | `false` | Different Types   |
| `[] == false`        | `true`  | JS Magic          |
| `[] === false`       | `false` | Object ≠ Boolean  |

---

# Interview Questions

1. What is Type Coercion?
2. Difference between `==` and `===`?
3. Why does `'5' + 3` return `"53"`?
4. Why does `'5' - 3` return `2`?
5. Why is `[] == false` true?
6. Why is `null == undefined` true?

---

# Interview One-Liner

Type Coercion is JavaScript's automatic conversion of one data type into another type during operations or comparisons.

---

# Key Takeaways

* ✅ Prefer `===` over `==`
* ✅ Understand coercion instead of memorizing outputs
* ✅ Avoid relying on weird coercion rules in production code
