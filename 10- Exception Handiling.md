## `try` and `except` keyword
they are used to prevent errors
```python 
try :
	line 1  
	line 2
except TypeError :
	line 1
	line 2
```

or we can write `except` without specifying TypeError in this case, any exception will be caught 
```python
try :
	line 1
	line 2
except :
	line 1
	line 2
```


==🔵Ex - 1==
```python
try :
	x = int(input("inter a number : "))
	y = int(input("inter second number : "))
	print(x//y)
	
except ValueError:
	print("Wrong input")
except :
	print("Try again")	
```

if user inputs string
```
Wrong input
```
if user inputs zero in the y 
```
Try again
```


