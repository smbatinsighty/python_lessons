# 12. modules

## Chapter 1
### 1. import
### 2. from
### 3. as
### 4. dir

![title](namespaces.png)



```python
# 1. import

# import math

# print(math.factorial(5))
# print(math.floor(3.9))
# print(math.ceil(3.1))

# import copy

# users = ["Lilit", "Aren", "Janna", "Samvel", "Gohar", "Armen", "Luiza"]
# copy_user = copy.deepcopy(users)
# print(copy_user)


# import random
# print(random.choice(users))
# print(random.randint(10, 100))

# dir(math) # return module's attributes


# import math
# import copy
# import random


# print(math.factorial(5))
# print(math.floor(3.9))
# print(math.ceil(3.1))

# users = ["Lilit", "Aren", "Janna", "Samvel", "Gohar", "Armen", "Luiza"]
# copy_user = copy.deepcopy(users)
# print(copy_user)

# print(random.choice(users))
# print(random.randint(10, 100))


# 2. from

# import copy.deepcopy # error
# from copy import deepcopy

# users = ["Lilit", "Aren", "Janna", "Samvel", "Gohar", "Armen", "Luiza"]
# copy_users = deepcopy(users)
# print(copy_users)


# 3. as

# import math as matьmatьika

# print(matьmatьika.factorial(5))
# print(matьmatьika.floor(3.9))
# print(matьmatьika.ceil(3.1))

# from copy import deepcopy as deepcopylist

# users = ["Lilit", "Aren", "Janna", "Samvel", "Gohar", "Armen", "Luiza"]
# copy_users = deepcopylist(users)
# print(copy_users)

# from math import *


# print(math.factorial(5)) # error because module imported with *
# print(factorial(5))
# print(floor(3.9))
# print(ceil(3.1))
```

### Chapter 2
### 1. create our module
### 2. create our package
