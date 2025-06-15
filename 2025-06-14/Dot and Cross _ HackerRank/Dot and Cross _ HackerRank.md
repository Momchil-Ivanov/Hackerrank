```
# Link = https://www.hackerrank.com/challenges/np-dot-and-cross/problem

import numpy

first_array = []
second_array = []

array_row_size = int(input())

for i in range(array_row_size):
    first_array.append(list(map(int, input().split(" "))))

for i in range(array_row_size):
    second_array.append(list(map(int, input().split(" "))))

A = numpy.array(first_array)
B = numpy.array(second_array)

result = numpy.dot(A, B)

print(result)
```