```
# Link = https://www.hackerrank.com/challenges/py-if-else/problem

import math
import os
import random
import re
import sys

if __name__ == '__main__':
    n = int(input().strip())
    
    if n % 2 != 0 or (n % 2 == 0 and 6 <= n <= 20):
        n = 'Weird'
    elif n % 2 == 0 and (2 <= n <= 5 or n > 20):
        n = 'Not Weird'

print(n)
```