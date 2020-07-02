# 17. regular expressions, exec, eval, pep

## Chapter 1
### 1. regular expressions intro
### 2. regular expressions methods
### 3. regular expressions operators


```python
# 1. regular expressions intro

# phone_number = input("please write your number")

# if phone_numer.find(...f):
#     print(f"number {phone_number} is valid")
# else:
#     print(f"number {phone_number} is not valid")

# import re

# 2. regular expressions methods

# match method

# reg_exp = 'test'
# email = 'test@gmail.com'

# match = re.match(reg_exp, email)
# print(match) # check with started
# if match is not None:
#     print(match.group(0)) # set position
# else:
#     print("not found")

# search method
# reg_exp = 'atest'
# email = 'atest@gmail.comatest'
# match = re.search(reg_exp, email)
# print(match.group(0)) # return first a
# print(match.group(0), match.start()) # start from 
# print(match.group(0), match.end()) # end in

# findall method

# reg_exp = 'a'
# email = 'atest@gmail.comatest'
# match = re.findall(reg_exp, email)
# print(match) # return list


# email = 'testA@gmail.com' # not found because email's A with upper case
# match = re.findall(reg_exp, email)
# print(match) # returna anum list

# ignore upper case and lower case 
# reg_exp = 'a'
# email = 'testA@gmail.com'
# match = re.findall(reg_exp, email, re.I) # re.I -> ignore
# print(match)

# split method

# split = re.split('-', 'a-b-c-d-e')
# print(split) # return splited list by regex

# split = re.split('-', 'a-b-c-d-e', maxsplit=2)
# print(split) 

# subn

# replace_with_regexp = re.subn('V', 'K', 'Vardan')

# print(replace_with_regexp)


# 3. regular expressions operators

# some_string = 'Hello world, my.  name is Vardan my firtname. is Vardanyan, I am 18 years old'
# find_all = re.findall(r'is', some_string) # find all substrings
# find_all = re.findall(r'[is]', some_string) # find i or s 
# find_all = re.findall(r'[^is]', some_string) # ^ find all execpt i or s
# find_all = re.findall(r'[a-z]', some_string) # find all lower case letters 
# find_all = re.findall(r'[A-Z]', some_string) # find all upper case letters 
# find_all = re.findall(r'[a-zA-Z]', some_string) # get all letters
# find_all = re.findall(r'[0-9]', some_string) # get all numbers
# find_all = re.findall(r'\d', some_string) # get all numbers 
# find_all = re.findall(r'[a-zA-Z0-9]', some_string) # get all numbers and letters
# find_all = re.findall(r'\w{1,}', some_string) # get letters where length >= 1
# find_all = re.findall(r'\w{3}', some_string) # devide 3 letters parts
# find_all = re.findall(r'\w{3} ', some_string) # devide 3 letters parts and space after 3 letters
# find_all = re.findall(r'\w{0,}', some_string) # get letters where length > 0 with spaces
# find_all = re.findall(r'\w+', some_string) # get letters where length >= 1 this exprestion = {1,}
# find_all = re.findall(r'\w*', some_string) # get letters where length > 0 this exprestion = {0,}
# find_all = re.findall(r'\w?', some_string) # get letters where length > 0 this exprestion = {0,1}
# find_all = re.findall(r'^\w+', some_string) # ^ =! not ^ == in begin string
# find_all = re.findall(r'\w+$', some_string) # $ string end
# \w == [a-zA-Z0-9]
# print(find_all)
# phone_number = input("please write your number")
# match = r'(\d{2,3}[-\.\s\(\)]??\d{3}[-\.\s]??\d{3})'

# if re.findall(match, phone_number):
#     print(f"number {phone_number} is valid")
# else:
#     print(f"number {phone_number} is not valid")
```

## Chapter 2
### 1. exec
### 2. eval


```python
# 1. exec

# code_by_string = 'a = 10\nprint("Square a is", a**2)'
# exec(code_by_string)
# import platform
# get_code_by_user = input('Write pytthon code here >>> ')
# exec(get_code_by_user)

# a = 5
# b = 'text'

# exec('print(a)', {})

# from math import *

# a = 5
# b = 'text'

# exec('print(dir())', {'a':a})

# def test():
#     a = 5
#     exec('print(a)', globals(), {'a':6})

# test()

# 2. eval

# program = '''5 + 10'''
# print(eval(program))

# program = '''5 + 10'''
# x = eval(program)
# y = exec(program)
# print(x)
# print(y)
```

## Chapter 3
### 1. pep


```python
# foo = my_func(arg1, arg2,
#               arg3, arg4)

# def my_func(
#         arg1, arg2, arg3,
#         arg4):
#     print(arg1)

# # or

# func_name = my_func(
#     'a', 'b', 'c',
#     'd', 'e', 'f',
# )

my_list = [
    1, 2, 3,
    4, 5, 6,
]

# # or

# my_list = [
#     1, 2, 3,
#     4, 5, 6,
#     ]


# with open('/path/to/some/file/you/want/to/read') as file_1, \
#          open('/path/to/some/file/being/written', 'w') as file_2:
#     file_2.write(file_1.read())

```
