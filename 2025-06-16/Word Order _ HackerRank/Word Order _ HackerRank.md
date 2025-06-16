```
# Link - https://www.hackerrank.com/challenges/word-order/problem?isFullScreen=false

number_of_words = int(input())

words_and_their_count_dict = {}

for i in range(number_of_words):
    word = input()
    if word in words_and_their_count_dict:
        words_and_their_count_dict[word] += 1
    else:
        words_and_their_count_dict[word] = 1

distinct_words = len(words_and_their_count_dict)
values = list(words_and_their_count_dict.values())

print(distinct_words)
print(" ".join(map(str, values)))
```