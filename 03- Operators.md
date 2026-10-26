### Arithmetic operators

| operators | name                   |
| --------- | ---------------------- |
| +         | addition               |
| -         | subtaction             |
| *         | multiplication         |
| **        | exponentiation (power) |
| /         | division               |
| //        | integer division       |
| %         | modulo                 |
### Comparison operator

| operators | name                  |
| --------- | --------------------- |
| ==        | equal                 |
| !=        | not equal             |
| >         | greater then          |
| <         | less then             |
| >=        | greater then or equal |
| <=        | less then or equal    |

### Logical operators


| operators | name |
| --------- | ---- |
| and       |      |
| or        |      |
| not       |      |
### identity operators


| operator | usage                            |
| -------- | -------------------------------- |
| is       | do tow thing refer to one object |
| is not   |                                  |
```python
a = [1,2,3]
b = a
c = [1,2,3]

print(a==b)
print(a==c)
 
print(a is b)
print(a is c)
```

```
True
True
True
False
```

### Membership operator

| operator | usage                                 |
| -------- | ------------------------------------- |
| in       | checks that the value in the variable |
| not in   |                                       |
```python
a = [1,2,3]

print(2 in a)
print(4 in a)
print(4 not in a)
```

```
True
False
True
```
