# 2.
## Chapter 1
### 1. Variables part 2
### 2. Reference (link)



```python
#1. Variables part 2

# reserved names (True, False, if, else ...etc)
# True = 7
# print(True)

# variable names cannot start with numbers
# 1_new_var ="some string"

# how assignment works
# x, y = "eggs", "spam"

# 2. Reference (link)
# x = 1
# y = x
# x = 7
# print(y)
```

## Chapter 2
### 1. Integer
### 2. Float


```python
# 1. Integer

# x = int()
# print(x)

# x = "7"
# int(x)
# print(type(x))
# x = int(x)
# print(type(x))

# 2. Float
# int to float
# print(float(10))

# float
# print(float(11.22))

# string to float
# print(float("-13.33"))

# white spaces ignored
# print(float("     -24.45\n"))

# error when we put string
# print(float("abc"))

# return float after devide
# print(10.2 / 2)

# return float after devide
# print(10 / 2.0)

# round(5.655, 2)
```

## Chapter 3
### 1. String sequence
### 2. String(double quotes, single quotes, special escape characters)
### 3. String format
### 4. String Methods


```python
# 1. Strings sequence

# x = asd # error

# some_text = "Hello world\nHow are you?" # /n
# some_text
# print(some_text)

# sequence
# some_text[0:7]
# print(some_text)

# find sequence length
# len(some_text)

# 2. String format

# name = "Vardan" 
# age = 27
# print("%s %d tarekana" % (name, age) )
# print("Hello, {0}. youe are {1}, {1}".format(name, age))
# print(f"Hello, {name}. youe are {age}, {age}, {age}") #available after python 3.6

# 3. String Methods
# x = str(55)
# print(x)
# some_text = "Hello World"

# print(some_text.lower())
# print(some_text.upper())

# some_text = "replaced_string"
# print(some_text)
# some_text = some_text.replace('replaced_string','new_string', 1)
# print(some_text)


# finded_string = some_text.find('p') # return dinded index or -1
# print(finded_string)
```
