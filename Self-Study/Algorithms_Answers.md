Exercise I

a)

Runtime: linear

This formuation is deceptive. The n cubed in the while conditional anchors your thinking high because n^3 is very large. But the increment step is also very large. For each iteration, our counter is incrementing by n^2. How many iterations are necessary to reach our end condition though? If our ceiling is n^3 and each step is n^2, dividing one from the other leaves us with the conclusion that it will take n steps of iteratively adding n^2 to reach n^3. Thus our runtime is linear, or O(n).

b)
