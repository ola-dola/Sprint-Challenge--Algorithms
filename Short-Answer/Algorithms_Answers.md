#### Please add your answers to the ***Analysis of  Algorithms*** exercises here.

## Exercise I

a) Runtime - O(log n)
 - The runtime increases slower than the rate of increase in n. This is because the value of a increases exponetianly on each iteration.
b) Runtime: O(n log n)
 - The runtime for increases slightly faster than the rate of increase in n. The "for loop" code part has a O(n), and the "while loop" has O(log n). Combination of which givesus the linearithmetric runtime of O(n log n).

```
sum = 0
for i in range(n):      # O(n)
    j = 1
    while j < n:
    j *= 2              # O(log n)
    sum += 1
```

c) Runtime: O(2^n) - Exponential

- The runtime increases at a much faster rate than the increase in n.

## Exercise II

- Start at n/2 floors. Drop an egg, see  if it breaks.
- If it breaks, start increasing by 1 to find the minimum floor required to break the eggs.
- If it doesn't break, start decreasing by 1.
- Repeat until the the floor at x+1 changes the behaviour(broken/unbroken)

Runtime => n/2 => O(n)
