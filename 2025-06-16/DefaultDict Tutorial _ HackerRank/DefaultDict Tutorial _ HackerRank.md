```
# Link - https://www.hackerrank.com/challenges/defaultdict-tutorial/problem?isFullScreen=false

first_group_count, second_group_count = list(map(int, input().split()))

first_group_name_and_position = {}

for i in range(1, first_group_count + 1):
    first_group_name_and_position[i] = input()

for i in range(second_group_count):
    second_group_name = input()
    if second_group_name in first_group_name_and_position.values():
        indexes = [key for key, value in first_group_name_and_position.items() if value == second_group_name]
        print(" ".join(map(str, indexes)))
    else:
        print(-1)
```