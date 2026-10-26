## inserting modules 


### 1- `import module1, module2,...`
when using the method of the module we have to write the name of module
like `module.method()`

```python
import random, math
print(math.sqrt(25))
print(random.random())
```

### 2- `import module as nickname`
when using the methods of the module we write the nickname of module 
like `nickname.method()`

```python
import random as r
print(r.randint(0,10))
```


### 3- `from module import method1, method2,...`
in this approach, the method's name is added directly to the current namespace
```python
from random import randint, randrange, random
print(randint(0,10))
print(random())
```


### 4- `from module import method as nickname`

```python
from random import randint as r
print(r(0,10))
```

### 5- `from module import *`
all method of module are added to the current namespace
> it is not recommended

```python
from random import *
print(randrange(0,10))
```