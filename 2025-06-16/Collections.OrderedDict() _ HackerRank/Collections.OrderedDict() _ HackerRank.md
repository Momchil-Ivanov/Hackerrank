```
# Link - https://www.hackerrank.com/challenges/py-collections-ordereddict/problem?isFullScreen=false

from collections import OrderedDict

nunmer_of_lines = int(input())

storage_dict = {}

for i in range(nunmer_of_lines):
    item = input().split()
    title = " ".join(item[:-1])
    price = int(item[-1])
    if title in storage_dict:
        storage_dict[title] += price
    else:
        storage_dict[title] = price

ordered_dict = OrderedDict(storage_dict.items())

for title, price in ordered_dict.items():
    print(title, price)
```