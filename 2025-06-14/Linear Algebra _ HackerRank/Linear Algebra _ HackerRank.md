```
# Link = https://www.hackerrank.com/challenges/np-linear-algebra/problem

import numpy
import math

count = int(input())
my_array = []

for i in range(count):
    coefficients = list(map(float, input().split(" ")))
    my_array.append(coefficients)

result = round(numpy.linalg.det(my_array), 2)
print(result)
```