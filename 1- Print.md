
# `Print(arg1, arg2, ... , argn)`
---
## Key word arg

> for each (,) one (space) will be typed
``` python
print(2,"Eqbal", end = "",sep = "")

```
> 2 and "Eqbal" is **arg**
> `end = ""` and `sep = ""`  is **key word arg** (it must always written after arg)
```run
2
Eqbal
```

---
### end = " "
It prevents the cursor from moving to another line 
we can also give input
```python
print("AB", end = "**")
print("X")
```

```run
AB**X
```

### sep = " "
instead of each (,) it will print whatever input we provide(give)
its default value is one space 
```python
print("AB", "C","D", sep = "**")
```

```run
AB**C**D
```

---

> if  we write an empty print() without any input it will print an empty line 
> it will not print a space 
> space a character though 

```python
print()
```

```run
```

---

## Special Characters 

special characters are predefined as string, and the system recognizes them 
از قبل تعریف شده هستن و به عنوان یک str هستن اما سیستم انها را میشناسد

### \n :    (new line)
it takes the cursor to another line

### \t :    (tab)
it make a tab (8 space or 4 space)

### \r : (return)
it takes the cursor to the first line
```python
print("Hello", "SS\rAA")
```

```
AAllo SS
```

---

## String Operators

### 1. (+)
```python
print("AB" + "CD")
```

```
ABCD
```

### 2. ( * )
```python
print("AB" * 3)
```

```
ABABAB
```

---


- [ ] print
- [ ] key word arg
- [ ] special character
- [ ] len()