```
# Link - https://www.hackerrank.com/challenges/collections-counter/problem?isFullScreen=false

number_of_shoes = int(input())
shoe_sizes = list(map(int, input().split()))
number_of_customers = int(input())
shoe_sizes_and_prices = {}
won_money = 0

for i in range(number_of_customers):
    shoe_size, price = map(int, input().split())
    if shoe_size in shoe_sizes:
        won_money += price
        shoe_sizes.remove(shoe_size)

print(won_money)
```