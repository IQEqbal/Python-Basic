## 1- bult in function
like : print(), len(), range(), ...

## 2- Made by user

```python
def function_name(arg1,arg2,...,argn):
	line 1
	line 2
```
> rule of naming function is like rule of naming variables 

==🔵 Ex -1 ==
```python
x = 3
y = 4
def myFunc(x,y):
	x += 3
	y -= 2
	p = x*y
	print(p)

myFunc(x,y)
print(x)
print(y)
print(p)
```

```
12
3
4
Traceback (most recent call last):
  File "c:\Users\Iqbal\Desktop\Python tuturial\app.py", line 12, in <module>
    print(p)
          ^
NameError: name 'p' is not defined
```

### `return` statement
it causes the function we created to produce an output
(it makes the function we created return a value)

```python
def square(a):
	return a**2
num = square(5)  # num = 25
```

### Local variable

### Global variable

