## `with` statement 

`with` statement automatically closes the file when the block ends

```python
with open( , ) as ObjName:
	line 1
	line 2
```

> we can assign to a variable the data of a file `x = f.read()`

```
text.txt
Hello;
```

```python
with open("text.txt","r") as f:
	x = f.read()	
print(x)
```

```
Hello;
```