```
# Link = https://www.hackerrank.com/challenges/np-inner-and-outer/problem

import numpy

first_array = []
second_array = []


first_array.append(list(map(int, input().split(" "))))
second_array.append(list(map(int, input().split(" "))))

inner_product = numpy.inner(first_array, second_array)
outer_product = numpy.outer(first_array, second_array)

print(inner_product.item())
print(outer_product)
```