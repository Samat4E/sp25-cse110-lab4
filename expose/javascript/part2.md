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
