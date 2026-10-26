## Variable 
it has many type
* int (integer)       
* float 
* bool (boolean)
* str (string)
*  ......
```python
_int = 4
_float = 3.4
_bool = True
_str = "Eqbal"

print(type(_int))
print(type(_float))
print(type(_bool))
print(type(_str))
```

```
<class 'int'>
<class 'float'>
<class 'bool'>
<class 'str'>
```

### Rules for naming variable

| True  | false |
| ----- | ----- |
| ab=5  | aB=5  |
| AB=5  | Ab=5  |
| ab2=5 | 2ab=5 |


---
### Iterable Variable
an object that contains a collection of elements that can be accessed one by one, allowing is to iterate over them using a *loop*
or 
they consist of a collection of elements that can be accessed sequentially, meaning we can also iterate over them in a loop 
like : *str, list, tuple, dict, set, ...*

```python
_str = "Eqbal"
for x in _str :
    print(x, end =" ")
```

```
E q b a l
```

---

## Combining variables in a string
### string = f" {var1} {var2}"
```python
a = "A"
b = "B"
c = f"{a} OK {b}"
print(c)
```

```
A OK B
```

---

## Methods of string

>In python everything is an object and each object has its own special functions that those functions called Methods  

### upper()
it converts all the letters in a string to uppercase
```python 
print("eqbal".upper())
```

```
EQBAL
```

### lower()
turns all the letters to lowercase 
```python
print("EQBAL".lower())
```

```
eqbal
```

### title()
turns first letter of each word to uppercase
```python
_str = "cyber security is perfect"
print(_str.title())
```

```
Cyber Security Is Perfect
```


### strip()
removes the spaces from the beginning and end
```python
_str = "   cyber security is perfect    "
print(_str.strip())
```

```
cyber security is perfect
```

### rstrip()
Right strip 

### lstrip()
left strip 

### find("a")
gives us the index of a
if a is not exist in the string it turns -1
if instead of a we write several character it gives as the first index of characters
```python
print("Eqbal".find("b"))
print("Eqbal".find("x"))
print("Eqbal".find("bal"))
print("Eqbal".find("byx"))
```

```
2
-1
2
-1
```

### replace("a" , "b")
replaces a and b in the string

---

variable 
combining variable in string
methods of string
