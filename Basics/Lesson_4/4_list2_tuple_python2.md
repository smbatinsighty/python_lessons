# 3. List part 2, Tuple, Python 2

## Chapter 1
### 1. Nested List
### 2. Deep and Shallow copy
### 3. id() function

```python
#1.Nested List

# numbers = [1, 2, 3]

# numbers[3]

# numbers[3] = 4

# nested_list = [1, 2, 3, ["10", 11, 12]]
# print(nested_list[3][0][1])

# users_tests = [
#     ["Lilit", "Aren", "Janna", "Samvel (Sam)", "Gohar", "Armen", "Luiza"],
#     [[1, 9, 8, 8, 7, 9, 8], [2, 9, 8, 8, 7, 9, 8], [7, 9, 8, 8, 7, 9, 8]]
# ]
# print(users_tests[1][2])

# 2. Deep and Shallow copy


# importing copy module 
# import copy 
  
# initializing list 1  
# li1 = [1, 2, [3, 5], 4] 

# li1 = [1, 2, [3, 5], 4] 
# li1_copy = li1.copy()
# li1_copy[2][0] = 1000

# x = 1    0, [1, 3, 4]

# print(li1)

# print(li1_copy)


# using copy for shallow copy

# li1_shallow_copy = copy.copy(li1)

# li1_shallow_copy[2][0] = 1000

# print(li1)
         
# print(li1_shallow_copy)

  
# # using deepcopy for deepcopy

# li1 = [1, 2, [3, 5], 4]

# li1_deep_copy = copy.deepcopy(li1)

# li1_deep_copy[2][0] = 1000

# print(li1)
         
# print(li1_deep_copy)
```

## Chapter 2
### 1. List Methods Part 2


```python
# list_of_strings = ['1','2','3','4']
# s = ", "
# s = s.join(list_of_strings)
# print(type(s))

# # split()
# x = 'vazgen@ chgnac dproc vorovhetev karatina'.split(" ", 2)
# print(x)
```

## Chapter 3
### 1. Touple


```python
# 1. Tuple
# x = tuple()
# print(x)

# x = (1, )
# print(type(x))
# x = (1, )
# print(type(x))

# thistuple = (1, 3, 7, 8, 7, 5, 4, 6, 8, 5)
# thistuple[1] = 1000
# x = thistuple.count(5)
# print(x)

# t1 = 1,
# print(t1)

# t2 = 1, 5,
# print(t2)

# t3 = 1, 5, 9
# print(t3)

# x = ('a','b', 5)
# var1 , var2, var3 = x
# print(var1, var2, var3)


# import timeit 
        
# x = timeit.timeit(stmt="[45,6,9,7,8,7,987,987,546]", number=1000000)
# y = timeit.timeit(stmt="(45,6,9,7,8,7,987,987,546)", number=1000000)
# print("list time " ,x)
# print("tuple time ", y)
```

## Chapter 4
### 1. Python2 VS Python3


```python
# Print in python2
# print 'hello' # 2.x

# print("hello") # 3.x


# print('hello', 'world', sep="\n", end=".") 
# print('hello', 'world', sep="\n", end=".") # 3.x



# Python 2
# 3 / 2 = 1
# 3 // 2 = 1
# 3 / 2.0 = 1.5
# 3 // 2.0 = 1.0

# Python 3
# 3 / 2 = 1.5
# 3 // 2 = 1
# 3 / 2.0 = 1.5
# 3 // 2.0 = 1.0

# long int in python 2
# x = 100L

# input
# 2.x -raw_input() # str
# input() # int

# 3.x-um menak input() u misht stringa veradarcnum
# #raw_input('enter a number: ')
# #x = input("enter a number")
# x = raw_input('hello')
# print(type(x)) (edited)
```
