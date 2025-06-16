```
# Link - https://www.hackerrank.com/challenges/py-collections-namedtuple/problem?isFullScreen=false

number_of_students = int(input())

columns = input().split()

marks_index = columns.index("MARKS")
total_marks = 0

for i in range(number_of_students):
    student = input().split()
    total_marks += int(student[marks_index])

average_marks = round(total_marks / number_of_students, 2)

print(f"{average_marks:.2f}")
```