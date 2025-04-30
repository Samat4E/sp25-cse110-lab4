### Part 2 – Questions

**1.** Line 12 will print `3`, because `var i` is function-scoped and accessible outside the `for` loop.

**2.** Line 13 will print the **last value of `discountedPrice`** calculated in the loop, because `var` makes it accessible outside the block.

**3.** Line 14 will print `150`, the last calculated `finalPrice`, which is still accessible because `var` was used in the outer scope.

**4.** The function returns `[50, 100, 150]` — each number is `50%` off the input prices.

**5.** Line 12 will cause a `ReferenceError` if `let i` was used instead of `var`, because `let` is block-scoped and not accessible outside the `for` block.

**6.** Line 13 will cause a `ReferenceError` if `let discountedPrice` was used, since it's block-scoped.

**7.** Line 14 will print `150` if `finalPrice` was declared with `var`, because it exists outside the loop too.

**8.** The function returns `[50, 100, 150]` — no error, logic is valid.

**9.** Line 11 will cause a `ReferenceError` if `let i` is used, because it's not accessible outside the loop block.

**10.** Line 12 will cause a `ReferenceError` if `let discountedPrice` is used, because it’s not accessible outside the loop.

**11.** The function returns `[50, 100, 150]` — all final prices are rounded and pushed to the result array correctly.

---

### Question 12

A. `student.name`  
B. `student["Grad Year"]`  
C. `student.greeting()`  
D. `student["Favorite Teacher"].name`  
E. `student.courseLoad[0]`

---

### Question 16 (see part2-question16.js)
/* 
for (let key in statistics) {
  if (key.startsWith('r') || statistics[key] % 2 === 1) {
    console.log(statistics[key]);
  }
}
*/

---

### Question 17

**Result:** `[2, 4, 6]`  
Explanation: Each element in the array `[1, 2, 3]` is passed to `doSomething(num)`, which multiplies it by 2. So:
- 1 × 2 = 2
- 2 × 2 = 4
- 3 × 2 = 6

---

### Question 18 (see part2-question18.js)
/*
setInterval(function() {
  let d = new Date();
  let time = d.toLocaleTimeString();
  console.log(time);
}, 1000);
*/

---

### Question 19

**Output:**  
1  
4  
3  
2

**Explanation:**  
- 1 prints immediately  
- 4 prints next (synchronous)  
- 3 is printed by the 0ms `setTimeout()` after the call stack clears  
- 2 prints after 1 second

---

### Type Conversion Results

- `'3' + 2` → `'32'` (string concatenation)
- `'3' - 2` → `1` (`'3'` converted to number)
- `3 + null` → `3` (`null` becomes 0)
- `'3' + null` → `'3null'` (string concatenation)
- `true + 3` → `4` (`true` becomes 1)
- `false + null` → `0` (`false` is 0, `null` is 0)
- `'3' + undefined` → `'3undefined'` (string + undefined)
- `'3' - undefined` → `NaN` (`'3'` becomes number, `undefined` becomes NaN)

---

### Comparison Results

- `'2' > 1` → `true` (`'2'` is coerced to number 2)
- `'2' < '12'` → `false` (string comparison)
- `2 == '2'` → `true` (loose equality, type coerced)
- `2 === '2'` → `false` (strict equality, different types)
- `true == 2` → `false` (true is 1, 1 ≠ 2)
- `true === Boolean(2)` → `true` (Boolean(2) is true, both are boolean `true`)

---

### Difference between == and ===

- `==` checks for **value equality** with **type coercion**  
- `===` checks for **strict equality** (same value and same type)
