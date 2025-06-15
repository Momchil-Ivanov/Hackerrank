```
# Link - https://www.hackerrank.com/challenges/nested-list/problem?isFullScreen=false

if __name__ == '__main__':
    n_value = int(input())
    my_dict = {}

    for i in range(0, n_value):
        name_value = input()
        score_value = float(input())

        my_dict[name_value] = score_value
    
    values_list = list(set(my_dict.values()))
    values_list.sort()
    second_lowest_score = values_list[1]
    
    key_array = []

    for key, value in my_dict.items():
        if value == second_lowest_score:
            key_array.append(key)
    
    key_array.sort()

    for key in key_array:
        print(key)
```