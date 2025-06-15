```
# Link = https://www.hackerrank.com/challenges/np-mean-var-and-std/problem

import numpy

my_array = []

row, col = map(int, input().split(" "))

for i in range(row):
    my_array.append(list(map(int, input().split(" "))))

my_array = numpy.array(my_array)

mean_axis_one = numpy.mean(my_array, axis = 1)
var_axis_zero = numpy.var(my_array, axis = 0)
std_axis_none = numpy.std(my_array, axis = None)

print(mean_axis_one)
print(var_axis_zero)
if std_axis_none == 0:
    print('{:.1f}'.format(std_axis_none))
else:
    print('{:.11f}'.format(std_axis_none))
```