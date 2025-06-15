```
# Link - https://www.hackerrank.com/challenges/list-comprehensions/problem?isFullScreen=false

if __name__ == '__main__':

    x_value = int(input())
    y_value = int(input())
    z_value = int(input())
    n_value = int(input())

    my_array = []

    for i in range(0, x_value + 1):
        for j in range(0, y_value + 1):
            for k in range(0, z_value + 1):
                if i + j + k != n_value:
                    my_array.append([i, j, k])

    my_array.sort()
    print(my_array)
```