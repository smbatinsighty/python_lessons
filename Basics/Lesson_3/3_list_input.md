# 3. Input, List
## Chapter 1
### 1. Help
### 2. Input


```python
#1. Help

# print(str.strip)
# print(help(str.strip)

# input()
# name = input()
# print(type(name))

# print("write your name ara!! please)")
# x = input()
# print(x)

# x = input("Please write your age")
# print(int(x))

# name = input("What's your name? ")
# print(name + "@ mer @ngerna" + "!")

```

## Chapter 2
### 1. List Introduction
### 2. Sequence
### 3. Mutable


```python
#1. List Introduction
# import random

# x = "Lilit"
# y = "Aren"
# z = "Luiza"
# a = "Janna"
# b = "Samvel" # (Samo)
# c = "Gohar"
# d = "Armen"
# print(x, y, z, a, b, c, d)


# x = list()
# x = []
# print(x)
# pythonists = ["Lilit", "Aren", "Janna", "Samvel (Samo)", "Gohar", "Armen", "Luiza"]
# ages = [60, 34, 62, 69, 63, 67, 61, "some string"]
# len(ages)
# pythonists[3] = "Vardan"
# print(pythonists)
# print(ages)


# 2. Mutable

# x = [1, 2, 3]
# y = x
# x[0] = 100
# print(y)

# 3. Sequence

# print(pythonists[0:])
# print(pythonists[-1])
# print(pythonists[:]) # copy
# print(pythonists[::-1]) # reverse
# print(pythonists[::1])

# print(pythonists + ages) # polimorfizm Introduction
# print(pythonists * 6)

# 3 in [1, 2, 3]

# print(random.choice(pythonists))
```

## Chapter 3
### 1. List methods
### 2. List functions


```python
## 1. List methods

# pythonists = ["Lilit", "Aren", "Aren", "Janna", "Samvel (Samo)", "Gohar", "Armen", "Luiza"]
# x = pythonists[0:3]


# x.append("Vardan") # add item to end of list
# name = pythonists.pop() # remove last item
# print(pythonists)
# print(x)

# help(list.pop)
# pythonists.insert(1, 'Vardan') # add in index
# pythonists.remove('Aren')
# pythonists.reverse()
# pythonists.sort(reverse=True)
# print(pythonists)

# 2. List functions

# x = [1, 2, 3, 4]
# print(sum(x))
# copy(x)
# len(x)
# x = sorted(x, reverse=True)
# print(x)
# list("abcd")
```
