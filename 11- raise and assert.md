## `raise` 

### 1- Usage 
it is used to raise a `RunTimeError`  

**syntax**-1
```python
raise TypeError
```
**syntax**-2
```python
raise TypeError ("Massage in the error")
```

==🔵Ex-1==
```python
print("Hello")
raise ValueError 
Print("Hi")
```

```
Hello
Traceback (most recent call last):
  File "c:\Users\Iqbal\Desktop\Python tuturial\app.py", line 2, in <module>
    raise ValueError
ValueError
```

### 2- Usage 
`raise` statement in `try-except` statement 
it raises the soonest error again

```python
try:
	x = 10/0
except:
	print("an error occurred")	
	raise
```

```
an error occurred
Traceback (most recent call last):
  File "c:\Users\Iqbal\Desktop\Python tuturial\app.py", line 2, in <module>
    x = 10/0
        ~~^~
ZeroDivisionError: division by zero
```

## `assert` 

`assert condition`
`assert condition, "Message"`
> if condition was `True` it will not run and doesn't raise error
> if condition was `False` it will run and raises an error called `AssertionError`

==🔵EX-1==
```python
try:
    age = int(input("Enter your age: "))
    assert age > 0
    print("you are ",age)
except:
    print("age can't be negative")
```
