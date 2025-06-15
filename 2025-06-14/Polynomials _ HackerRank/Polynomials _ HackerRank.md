```
# Link = https://www.hackerrank.com/challenges/np-polynomials/problem

import numpy as np

coefficients = list(map(float, input().split(" ")))
x_value = float(input())
result = np.polyval(coefficients, x_value)
print(result)
```