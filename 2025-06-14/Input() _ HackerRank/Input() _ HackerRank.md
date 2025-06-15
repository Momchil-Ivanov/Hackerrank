```
# Link = https://www.hackerrank.com/challenges/input/problem

a, b = map(int, input().split())
poly_str = input().strip()
def evaluate_poly(poly, x):
    try:
        # Replace 'x' with the value and evaluate
        code = poly.replace('x', str(x))
        return eval(code)  # Evaluates the expression
    except:
        return None  # Return None if evaluation fails

result = evaluate_poly(poly_str, a)
if result is not None and result == b:
    print(True)
else:
    print(False)
```