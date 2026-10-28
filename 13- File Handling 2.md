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

## Methods of File .......ii

### 1- `read()`
it is used to read the file 

### 2- `write()`
it is used to write in to file
##### EX-1
```python
f = open("text.txt","w")
f.write("Hello")
f.close()
```

```
text.txt
Hello
```

### 3- `close()`
it cuts the connection between the object and the file

### 4- `tell()`
it return the position of `File Handle`

##### EX-1
```
text.txt
Hello world!
```

```python
f = open("text.txt","r")
f.read(4)
print(f.tell())
```

```
4
```

### 5- `seek(a)`
it is used to change the position of `File Handle`

##### EX-1
```
Hello werld!
welcome 
```

```python
f = open("text.txt","r")
f.seek(7)
print(f.read())
```

```
erld!
welcome
```
### 6- `readline()`
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
### 7- `readlies()`
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



## Mode .......ii

> BoF: Beginning of File
> EoF: End of File


| Mode   | Description     | Position of File Handle |
| ------ | --------------- | ----------------------- |
| `"r"`  | Read            | BoF                     |
| `"w"`  | Write           | BoF                     |
| `"a"`  | Append          | EoF                     |
| `"r+"` | Read and write  | BoF                     |
| `"w+"` | Write and read  | BoF                     |
| `"a+"` | Append and read | EoF                     |

### `"r+"`
it starts writing from the current position of the `File Handle`
if `File Handle` was on a character and then we write our new text overwrites on the existing text

when we use `read()` and then use `write()` Python can't get the position of `File Handle`
because of this it appends instead of overwriting or writing
the solution is after used `read()` we must use
`f.seek(f.tell))`
##### EX-1
```
text.txt
Hello world;
Software Engineering
```

```python
f = open("text.txt","r+")
print(f.readline())
f.write("welcome to Cybersecurity")
f.close()
```

```
text.txt
Hello world;
Software Engineeringwelcome to Cybersecurity
```

##### EX-2
```
text.txt
Hello world;
Software Engineering
```

```python
f = open("text.txt","r+")
print(f.readline())
f.seek(f.tell())
f.write("welcome to Cybersecurity")
f.close()
```

```
text.txt
Hello world;
welcome to Cybersecurity
```



### `"w+"`
first it deletes all of data in file then we can read and write 
in reading and writing we must spot the position of `File Handle`

```
text.txt
Hello world;
Software Engineering
```

```python
f = open("text.txt","w+")
print(f.read())
f.write("wlcome in Cyber security")
f.seek(0)
print(f.read())
```

```

wlcome in Cyber security
```


### `"a+"`
for reading the position of `File Hanlde` is considered but 
for writing the position of `File Hanlde` is not considered 
