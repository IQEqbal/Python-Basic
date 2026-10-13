# `_list = [a,b,c, ... ,n] `

`list` is an iterable variable that stores multiple item in sequence
each item has an index

to access or modify (change) each item, we cam use square brackets [ ]

```python
_list = [1,2,3,"eqbal",5]

print(_list[1])

print(_list)
_list[0] = "cyber"  
print(_list)
```

```
2
[1, 2, 3, 'eqbal', 5]
['cyber', 2, 3, 'eqbal', 5]
```


## Methods of List

### 1 - append()             `nameObj.append(a)`
to add a value to end of a list
that value adds in the son of list

```python
_list = [1,3,4,5]
_list.append(6)
# [1,3,4,5,6]
```

### 2- insert( , )             `nameObj,insert(index,a)`
to insert a value at a specific index 
(to add a value in to a desire index)

```python
_list = [1,3,4,5]
_list.(1,"Eqbal")
# [1,"Eqbal",4,5]
```

### 3- remove()         `nameObj.remove(a)`
to remove a value from a list
if a value appears multiple times, it removes the first occurrence of that value
اگر از ان مقدار زیاد بود نزدیکتزن اندکس را حذف میکند نه تمام انرا

```python
_list = [1,2,2,2]
_list.remove(2)
# [1,2,2]
```

### 4- index()           `nameObj.index(a)`
it returns the index of  the value that we inserted

```python
_list = [1,2,3,4]
print(_list.index(3))
```

```
2
```
