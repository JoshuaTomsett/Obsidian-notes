[[ECM1400 Programming]]

14-Oct-2022

### With

``` python
with open(filename) as f:
	word_list.append(word) for word in f.read()
```

with can be used to control the scope of an object
here the file will be closed once the with statement has finished, which will save memory

### Unknown and unlimited arguments

##### args

`*args` : can be used to define an unknown number of arguments

```python
def func(*args):
	print(args)
	for value in args:
		print(value)
```
![[Pasted image 20221014105758.png]]

inside the function args is a tuple of the passed values

##### Kwargs

`**kwargs` can be used to pass unknown keyword arguments to a function ( a = 5)

```python
def func(**kwargs):
	print(kwargs)
```
![[Pasted image 20221014110311.png]]

inside the function kwargs is a dictionary

### Default arguments

```python
def func(a , b = 0):
```

- a value must be passed for a
- but passing a value for b is optional and will default to the specified value if no other value is given