### Part 1 – Questions

**1.** `values added: 20` will be printed. `var` is function-scoped, so `result` is accessible outside the `if` block.

**2.** `final result: 20` will be printed. Again, `var` makes `result` available in the entire function.

**3.** We should not use `var` because it is function-scoped and can lead to bugs due to hoisting or accidental reuse of variable names.

**4.** `values added: 20` will be printed using `let`, which is block-scoped and works fine inside the `if` block.

**5.** Line 13 will cause an error because `let result` is not accessible outside the block where it was defined (`if` block only).

**6.** Line 7 will throw a `TypeError` because `const result = 0` means the variable can't be reassigned. The next line tries to reassign it.

**7.** Line 13 will cause a `ReferenceError` because `result` is block-scoped and can't be accessed outside the `if` block.
