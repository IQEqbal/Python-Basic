### Concept of `File Handle` and `read(a)` method
we can specify how many characters the `read()` method should read by passing an argument to it
if we pass another argument, it reads the next characters instead of reading the previous ones again

**But why?** because there is a thing called `File handle` the `read()` method any character reads file handling counts it and when it reads 2 character `File handle` goes 2 character and when we again call `read()` it starts reading from 2nd character because `File handle` starts from 2nd character 

```
text.txt
Hello, world.
welcome.
```

```python
f = open("text.txt","r")     # File Handing = 0
print(f.read(4))             # File Handing = 4
print(f.read(2))             # File Handing = 6
print(f.read())              # File Handing = 21
print(f.read())              # it doesn't read becouse File handling is in the end
```

```
Hell
o,
 world.
welcome.

```

## Methods of File
### `write()`


### `close()`
it cuts the connection between the object and the file

### `tell()`
it return the position of `File Handle`

### `seek(a)`
it is used to change the position of `File Handle`

### `readline()`
it reads a line of file 
if the `File Handle` is at the beginning of a line, it reads all the characters in that line 
if it is in the middle of a line, it reads from that position to the end of the line
in other word it reads until `\n` reaches

##### EX-1
```
text.txt
Hello, world
welcome
How are you
```

```python
f = open("text.txt"."r")
print(f.readline())
```

```
Hello, world

```
### `readlies()`
it puts each line in a `list` item 
or other word it converts each line into a `list` item

##### EX-1
```
text.txt
Hello, world
welcome
How are you
```

```python
f = open("text.txt","r")
print(f.readlines())
```

```
['Hello, world\n', 'welcome\n', 'How are you']
```


















