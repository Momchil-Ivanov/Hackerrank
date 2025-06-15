```
# Link - https://www.hackerrank.com/challenges/find-second-maximum-number-in-a-list/problem?isFullScreen=false

if __name__ == '__main__':
    n_value = int(input())
    my_array = list(map(int, input().split()))
    unique_array = sorted(list(set(my_array)), reverse=True)
    runner_up_score = unique_array[1] # 2nd highest score
    print(runner_up_score)
```