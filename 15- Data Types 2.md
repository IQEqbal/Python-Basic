
#### Index Based Data Types
indexable object are objects whose elements can be accessed using an index
> like: `str`, `list`, `tuple`, ...

#### Key based Data Types
keyable object are objects that elements can ne accessed with using key 
> like: `dict`


## `None`
it takes the lowest memory

```python
x = None
print(type(x))
print(x)
```

```
<class 'NoneType'>
None
```

## `dict`

`_dict = {A:a, B:b,..., N:n}`
> N: key
> n: value

dictionary is an `iterable varibale` and key based
if several value have a same kay 

```python
x = {"A":5, "B":10, "C":15, "A":3}

print(x)
print(x["A"])

# to print keys
for i in x:
    print(i)

# to print values
for i in x:
    print(x[i])
```

```
{'A': 3, 'B': 10, 'C': 15}
3
A
B
C
3
10
15
```

### to append in `dict`
```python
x = {"A":5, "B":10, "C":15}
x["D"] = 20
```

### `del` statement 
to delete value from a `dict`
```python
x = {"A":5, "B":10, "C":15}
del x["B"]
print(x)
```

```
{'A': 5, 'C': 15}
```

## `tuple`

`_tuple = (val1, val2,..., valn)`

it is like `list`
tuple is an `Iterable variable` and index based
we can not change it's size after declare 
we can declare a `tuple` two time 

```python
x = (1,2,3)
print(x[0])
print(x)

x = (4,5)
print(x)
# x[0] = 6   TypeError
```

```
1
(1, 2, 3)
(4, 5)
```

## `set`

`_set = {val1, val2, ... ,valn}`

it is like `dict` but it is index based 
and also it is `iterable variable` but we can't access to a specific index
we can access to it's indexes with using `for` loop and can `print`

we can't append an index into it, and we can't change an index of value
if we add a value that already exists in the `set`, the value doesn't add to it
**(A `set` does not allow duplicate value)**

> `set` and `dict` work based on Hash table

##### EX-1
```python
x = {1,2,3}
x[0] = 1
```

```
  File "c:\Users\Iqbal\Desktop\Coding\Python codes\app.py", line 2, in <module>
    x[0] = 1
    ~^^^
TypeError: 'set' object does not support item assignment
```

##### EX-2
```python
x = {1,2,3}

for i in x:
	print(i,end="")
```

```
123
```

##### EX-3
```python
x = {1,2,3,1}
print(x)
```

```
{1,2,3}
```



