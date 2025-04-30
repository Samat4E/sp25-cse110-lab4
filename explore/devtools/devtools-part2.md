## devtools-part2.md

**1. What was the bug?**  
The bug was that the inputs `num1` and `num2` were being added as strings instead of numbers. So instead of calculating the correct sum, it was joining the two strings together (e.g., "2" + "3" = "23").

**2. How would you fix it?**  
To fix the bug, I converted both inputs to numbers using `Number()`.  
The new line of code is:

```js
let result = Number(num1) + Number(num2);
