```
JAVASCRIPT TYPE COERCION
═══════════════════════════════════════════════

WHAT IS TYPE COERCION?
─────────────────────
Type Coercion means JavaScript automatically converts one data type into another type to perform an operation.

GOLDEN RULES
────────────
==  → Checks value only (JavaScript converts types)
=== → Checks value + type (No conversion)

+ with string → Concatenation
-, *, /, %    → Convert to Number


1. '5' + 3
──────────
Output:   "53"
Why?      String + Anything = String
Internal: '5' + '3'
Real:     "House No: " + 5  →  "House No: 5"
Trick:    String + Anything = Join


2. '5' - 3
──────────
Output:   2
Why?      Math operators convert strings to numbers
Internal: 5 - 3
Trick:    - * / % = Number Conversion


3. '5' == 5
───────────
Output:   true
Why?      Loose equality checks value only
Internal: 5 == 5
Trick:    == → Value Only


4. '5' === 5
────────────
Output:   false
Why?      Strict equality checks value and type
Trick:    === → Value + Type


5. null == undefined
────────────────────
Output:   true
Why?      Special JavaScript rule
Trick:    Best Friends 🤝


6. null === undefined
─────────────────────
Output:   false
Why?      Different types
Trick:    Best Friends with Different ID Cards 😄


7. [] == false
──────────────
Output:   true
Why?      false → 0, [] → '' → 0, then 0 == 0
Trick:    JS Magic 🪄


8. [] === false
───────────────
Output:   false
Why?      [] → Object, false → Boolean, Different types
Trick:    Object ≠ Boolean


FINGER-TIP REVISION
═══════════════════
Code            │ Output │ Trick
────────────────┼────────┼──────────────────
'5' + 3         │ "53"   │ String Joins
'5' - 3         │ 2      │ Number Conversion
'5' == 5        │ true   │ Value Only
'5' === 5       │ false  │ Value + Type
null == undef   │ true   │ Best Friends
null === undef  │ false  │ Different Types
[] == false     │ true   │ JS Magic
[] === false    │ false  │ Object ≠ Boolean


INTERVIEW QUESTIONS
═══════════════════
• What is Type Coercion?
• Difference between == and ===?
• Why does '5' + 3 return "53"?
• Why does '5' - 3 return 2?
• Why is [] == false true?
• Why is null == undefined true?


ONE-LINER
═════════
Type Coercion is JavaScript's automatic conversion of one data type into another type during operations or comparisons.


KEY TAKEAWAYS
═════════════
✅ Prefer === over ==
✅ Understand coercion instead of memorizing outputs
✅ Avoid relying on weird coercion rules in production code
```
