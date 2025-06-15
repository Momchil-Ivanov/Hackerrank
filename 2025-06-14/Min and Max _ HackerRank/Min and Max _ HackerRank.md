```
# Link = https://www.hackerrank.com/challenges/np-min-and-max/problem

import numpy

my_array = []

row, col = map(int, input().split(" "))

for i in range(row):
    my_array.append(list(map(int, input().split(" "))))

my_array = numpy.array(my_array)

min_array = numpy.min(my_array, axis = 1)
print(numpy.max(min_array))
```