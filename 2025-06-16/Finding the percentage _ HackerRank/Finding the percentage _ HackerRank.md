```
# Link - https://www.hackerrank.com/challenges/finding-the-percentage/problem?isFullScreen=false

if __name__ == '__main__':
    n_value = int(input())
    my_dict = {}

    for i in range(0, n_value):
        current_student = list(map(str, input().split()))
        name_value = current_student[0]
        score_values = list(map(float, current_student[1:]))
        average_score = round(sum(score_values) / len(score_values), 2)

        my_dict[name_value] = average_score

    chosen_student = input()
    print(f"{my_dict[chosen_student]:.2f}")
```