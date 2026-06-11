JavaScript Type Coercion
What is Type Coercion?
Type Coercion means JavaScript automatically converts one data type into another type to perform an operation.
Golden Rules
== → Checks value only (JavaScript converts types)
=== → Checks value + type (No conversion)
+ with string → Concatenation
-, *, /, % → Convert to Number
1. '5' + 3
JavaScript
'5' + 3
Output:
JavaScript
"53"
Why?
String + Anything = String
Internally:
JavaScript
'5' + '3'
Real Life:
JavaScript
"House No: " + 5
// "House No: 5"
Memory Trick:
String + Anything = Join
2. '5' - 3
JavaScript
'5' - 3
Output:
JavaScript
2
Why?
Math operators convert strings to numbers.
Internally:
JavaScript
5 - 3
Memory Trick:
/ % = Number Conversion
3. '5' == 5
JavaScript
'5' == 5
Output:
JavaScript
true
Why?
Loose equality checks value only.
Internally:
JavaScript
5 == 5
Memory Trick:
== → Value Only
4. '5' === 5
JavaScript
'5' === 5
Output:
JavaScript
false
Why?
Strict equality checks value and type.
Memory Trick:
=== → Value + Type
5. null == undefined
JavaScript
null == undefined
Output:
JavaScript
true
Why?
Special JavaScript rule.
Memory Trick:
Best Friends 🤝
6. null === undefined
JavaScript
null === undefined
Output:
JavaScript
false
Why?
Different types.
Memory Trick:
Best Friends with Different ID Cards 😄
7. [] == false
JavaScript
[] == false
Output:
JavaScript
true
Why?
JavaScript internally converts:
false → 0
[] → '' → 0
Then:
0 == 0
Memory Trick:
JS Magic 🪄
8. [] === false
JavaScript
[] === false
Output:
JavaScript
false
Why?
[] → Object
false → Boolean
Different types.
Memory Trick:
Object ≠ Boolean
Finger-Tip Revision
Code
Output
Memory Trick
'5' + 3
"53"
String Joins
'5' - 3
2
Number Conversion
'5' == 5
true
Value Only
'5' === 5
false
Value + Type
null == undefined
true
Best Friends
null === undefined
false
Different Types
[] == false
true
JS Magic
[] === false
false
Object ≠ Boolean
Interview Questions
What is Type Coercion?
Difference between == and ===?
Why does '5' + 3 return "53"?
Why does '5' - 3 return 2?
Why is [] == false true?
Why is null == undefined true?
Interview One-Liner
Type Coercion is JavaScript's automatic conversion of one data type into another type during operations or comparisons.
Key Takeaways
✅ Prefer === over ==
✅ Understand coercion instead of memorizing outputs
✅ Avoid relying on weird coercion rules in production code :::
