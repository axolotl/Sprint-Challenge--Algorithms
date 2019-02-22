Exercise I

a)

Runtime: linear

This formuation is deceptive. The n cubed in the while conditional anchors your thinking high because n^3 is very large. But the increment step is also very large. For each iteration, our counter is incrementing by n^2. How many iterations are necessary to reach our end condition though? If our ceiling is n^3 and each step is n^2, dividing one from the other leaves us with the conclusion that it will take n steps of iteratively adding n^2 to reach n^3. Thus our runtime is linear, or O(n).

b)

Runtime: quadratic

Here we have 4 nested loops, the outer 3 of which are iterating on n. The second and third loops are iterating on n - 1 and n - 2 respectively, but this is hardly significant for very large n's, so we can simplify and say that they are each iterating on n. The fourth loop, by contrast, will always iterate over ten items, no matter how large k gets. This is therefore constant and we can drop it from the runtime. Thus we are left with a runtime of O(n^3).

c)

Runtime: linear

For each time the function recurs, the input value is reduced by one. And when the input value reaches zero, the function will stop recuring. The function will thus run a number of times that is equal to the input value, making the runtime O(n).

Exercise II

The plan to zero in on floor _f_ involves maximizing the number floors that _f_ is not for each egg we drop. So we start at the middle floor and drop an egg. If it breaks, we know that _f_ must be on the lower half of the building. So then we move to the middle of that section and drop an other egg. In each step, we cut the remaining possible floors in half, drop an egg, and see if the middle value is too high or too low. In this way we will arrive at floor _f_ in O(log(n)) steps.
