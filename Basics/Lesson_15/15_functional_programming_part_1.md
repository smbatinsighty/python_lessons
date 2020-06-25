# 15. functional programming part 1

## Chapter 1
### 1. lambda


```python
### 1. lambda


# some_function = lambda x: x**2
# print(some_function(3))

# print((lambda x: x**2)(6))

# def f1(get_square):
#     square = get_square(2)
#     print(square)
    


# f1(lambda x: x**2)
# f1(lambda x: x**3)
# f1(lambda x: x**4)

# price = ""
# while not price or price == "":
#     price = input("please write price: ")
    
# price = int(price)
# # full_price = price + (price * 24) / 100
# cost = {
#     "price": price,
# #     "full_price": full_price,
#     "full_price": (lambda x: x + (x * 24) / 100)(price)
# }

# print(cost)

# def show(show_user):
#     product = {"product": "chaynik", "price": 50000}
#     print(show_user(product))

# show(lambda product : product["price"] + 2000 if product["price"] > 100000 else product["price"] + 1000)

# numbers = [
#     lambda x: x**2, 
#     lambda x: x**3, 
#     lambda x: x**4
# ]

# for f in numbers:
#     print(f(2))    # 4, 8, 16

# print(numbers) # 9 
# print(numbers[0](3)) # 9 

# x = (lambda *args: args)
# print(x(1, 2, 3, 4))

# def knights():
#     title = 'Sir'
#     action = (lambda x: title + ' ' + x)
#     return action

# act = knights()

# print(act("Robin"))
```

## Chapter 2
### 1. zip
### 2. map


```python
# 1. zip

# print(list(zip([1, 2, 3], "abc")))

# numbers = [1, 2, 3, 4]

# def int_to_str(numbers):
#     str_numbers = []
#     for number in numbers:
#         str_numbers.append(str(number))
#     return str_numbers

# print(int_to_str(numbers))
# print(numbers)
# 2. map

# numbers = [1, 2, 3, 4]
# print(str)
# str_numbers = map(str, numbers)
# print(list(str_numbers))

# str_numbers = int_to_str(numbers)


# print(str_numbers)

# def change_item(arg):
#     return str(arg) + '-is changed'

# L = [1, 2, 3, 'item1', 'item2']
# map_object = map(change_item, str(L)) # return map object
# print(list(map_object))

# def change_item(arg): # add second parameter
#     return str(arg) + '-is changed' 

# L = [1, 2, 3, 'item1', 'item2']

# map_object = map(change_item, L) # return map object

# print(list(map_object)) # we can change to any type

# next(map_object)

# for item in map_object:
#     print(item)

# L = [1, 2, 3, 'item1', 'item2']

# map_object = map(lambda x: str(x) + " is changed", L)

# for item in map_object:
#     print(item)

# numbers = [1, 2, 3, 4]
# def get_square(numbers):
#     new_list = []
#     for number in numbers:
#         new_list.append(number ** 2)
#     return new_list
        

# def get_cube(numbers):
#     new_list = []
#     for number in numbers:
#         new_list.append(number ** 3)
#     return new_list
        
# def incr_number(numbers):
#     new_list = []
#     for number in numbers:
#         new_list.append(number + 1)
#     return new_list

# squares = get_square(numbers)
# cubes = get_cube(numbers)
# increments = incr_number(numbers)
# print("---------with functions-----------")
# print(squares)
# print(cubes)
# print(increments)
# squares = map(lambda x: x ** 2, numbers)
# cubes = map(lambda x: x ** 3, numbers)
# increments = map(lambda x: x + 1, numbers)
# print("---------with map----------------")
# print(list(squares))
# print(list(cubes))
# print(list(increments))
```

## Chapter 3
### 1. filter
### 2. reduce


```python
# def less_than_five(arg):
    
#     return arg > 5

# sequence = [1, 2, 3, 22, 4, 5, 6, 33, 7, 8, 9, 10, 4]

# filtered_seq = filter(less_than_five, sequence) # why map, generator ...etc not return list

# print(list(filtered_seq)) 

# def find_a(some_text):
#     return "l" == some_text


# some_text = 'hello world'

# filtered_seq = filter(find_a, some_text)

# print(len(tuple(filtered_seq)) # print length

# some_text = 'hello world'

# filtered_seq = filter(lambda x: x == 'l', some_text)

# print(tuple(filtered_seq))


# 2. reduce

# from functools import reduce

# numbers = [1, 2, 3, 4, 5]

# def custom_sum(first, second):
#     print(first, second, sep="||") # 1, 2 | 3, 3 
#     return first + second
#     return 20 + second

# result = reduce(custom_sum, numbers)
# print(result)

# numbers = [1, 2, 3, 4, 5]

# def custom_sum(first, second):
#     print(first, second, sep="||")
#     return first + second

# result = reduce(custom_sum, numbers, 10)
# print(result)
```
