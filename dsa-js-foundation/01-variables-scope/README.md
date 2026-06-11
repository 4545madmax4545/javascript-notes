# JavaScript Variables & Scope

## What is a Variable?

A variable is a container used to store data.

Example:

```js
let name = "Jalil";
```

---

# var vs let vs const

| Feature | var | let | const |
|----------|----------|----------|----------|
| Scope | Function | Block | Block |
| Redeclare | ✅ Yes | ❌ No | ❌ No |
| Reassign | ✅ Yes | ✅ Yes | ❌ No |
| Hoisting | ✅ Yes | ✅ Yes (TDZ) | ✅ Yes (TDZ) |

---

## var

### Example

```js
var age = 25;
var age = 30;

console.log(age);
```

Output:

```js
30
```

### Real Life

School register-la old value mela new value overwrite panra maari.

---

## let

### Example

```js
let city = "Madurai";

city = "Chennai";

console.log(city);
```

Output:

```js
Chennai
```

### Real Life

Phone wallpaper maathura maari value change panna mudiyum.

---

## const

### Example

```js
const country = "India";

console.log(country);
```

Output:

```js
India
```

### Real Life

Date of Birth maari.
Change panna mudiyadhu.

---

# Block Scope

Variables inside {} only work inside that block.

Example:

```js
{
 let x = 10;
}

console.log(x);
```

Output:

```js
ReferenceError
```

### Real Life

Bedroom key bedroom-ku mattum.

Outside use panna mudiyadhu.

---

# Function Scope

Example:

```js
function test() {
 var y = 20;
}

console.log(y);
```

Output:

```js
ReferenceError
```

### Real Life

Office ID card office-kulla mattum work aagum.

---

# Hoisting

JavaScript declarations are moved to top before execution.

Example:

```js
console.log(a);

var a = 10;
```

Output:

```js
undefined
```

Actual:

```js
var a;

console.log(a);

a = 10;
```

---

# Temporal Dead Zone (TDZ)

Using let or const before declaration causes error.

Example:

```js
console.log(b);

let b = 20;
```

Output:

```js
ReferenceError
```

---

# Interview Questions

## Q1. Difference between var let const?

Answer:

var → Function scoped

let → Block scoped

const → Block scoped and cannot be reassigned

---

## Q2. What is Block Scope?

Answer:

Variable exists only inside {}.

---

## Q3. What is Function Scope?

Answer:

Variable exists only inside function.

---

## Q4. What is Hoisting?

Answer:

JavaScript moves declarations to the top before execution.

---

## Q5. What is TDZ?

Answer:

Accessing let or const before initialization.

---

# Key Takeaways

✅ Prefer const by default

✅ Use let when value changes

✅ Avoid var in modern JavaScript

✅ Understand scope before learning closures
