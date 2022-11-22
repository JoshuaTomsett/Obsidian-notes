[[ECM1400 Programming]]

17-Nov-2022


A function that calls itself, e.g: factorial function below

```python
def factorial(num):
	if num == 0:
		return 1
	else:
		return num * factorial(num - 1)
```

