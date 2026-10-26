> **text file :** the data is stored as text

> **Binary file :** the data is stored as binary codes

> we can create a text file in the IDE with `.txt` extension

### `open("address", mode)`

`var = open("address", mode)`  
var become an object


## Methods of File

### `read()`
it used to read the data of file
#### EX-1
```text.txt
text.txt
Hello;
```

```python
f = open("text.txt","r")
print(f.read())
print(f)
```

```
Hello;
<_io.TextIOWrapper name='test.txt' mode='r' encoding='cp1252'>
```


## Mode 
> the way open a file

### `"r"` (read)
it is default mode of `open` function
#### EX-1
```text.txt
text.txt
Hello;
```

```python
f = open("text.txt","r")
print(f.read())
print(f)
```

```
Hello;
<_io.TextIOWrapper name='test.txt' mode='r' encoding='cp1252'>
```

### `"w"` (write)
it is used to write in a file 
we can't read a file with this mode
previous data will delete from the file
if we open a file which doesn't exist, the system will crate a file with that name

#### EX-1
```
text.txt
Hello;
```

```python
f = open("text.txt","w")
print(f.read())
```

```
Traceback (most recent call last):
  File "c:\Users\Iqbal\Desktop\Coding\Python codes\app.py", line 2, in <module>
    print(f.read())
          ~~~~~~^^
io.UnsupportedOperation: not readable
```
#### EX-2
```
text.txt
Hello;
```

```python
f = open("text.txt","w")
f.write("Hi Eqbal \nHow are you")
f.close()
```

```
text.txt
Hi Eqbal 
How are you
```


### `a` (append)
it is used to append(add) data to the end of a file

#### EX-1
```
text.txt
Hello;
```

```python
f = open("text.txt","a")
f.write("Eqbal \nHow are you")
f.close()
```

```
text.txt
Hello;Eqbal 
How are you
```



