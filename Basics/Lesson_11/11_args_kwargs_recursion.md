# 11. args, kwargs, recursion

## Chapter 1
### 1. args
### 2. kwargs


```python
### 1 args
# first_name = "Gago"
# last_name = "Adunc"

# def f(first_name, last_name, test_1, test_2, test_3):

#     print(first_name, last_name, test_1, test_2, test_3)

# f(first_name, last_name, 1, 2, 3)

# f(first_name, last_name, 1, 2, 3, 4)

# def f(first_name, last_name, *args):
    
#     print(first_name, last_name, args)
    
# f(first_name, last_name, 1, 2, 3)

# f(first_name, last_name, 1, 2, 3, 4)



# def func(a, b, c, d): print(a, b, c, d)

# args = (1, 2)
# args += (3, 4)
# print(*args)
# print(1, 2, 3, 4)

# func(*args)

# func(*'abcd')

# def func(*args, e): print(args, e)
# func(*'abcd', 8) # show with keyword argument

# 2. kwargs

# def f(**kwargs): 
#     print(kwargs)
# f(a=1, b=2, c=3)

# def f(a, *args, **kwargs): 
#     print(a, args, kwargs)
#     print(type(a), type(args), type(kwargs))
    
# f(1, 2, 3, x=1, y=2)

# def func(a, b, c, d): 
#     print(a, b, c, d)

# kwargs = {'a': 1, 'b': 2, 'c': 3}
# kwargs['d'] = 4

# print(**kwargs) # a= 1 ...

# func(**kwargs)
# func(a=1, b=2, c=3, d=4)
```

## Chapter 2
### 1. recursion


```python
# def make_matryoshka(n):
#     if n == 1:
#         print("matryoshka")
#     else:
#         print("matryoshkayi verevi mas", n)
#         make_matryoshka(n-1)
#         print("matryoshkayi nerqevi mas", n)
    
# make_matryoshka(5)
# def func1(x):
#     print(x)
#     func1(x + 1)

# func1(1)

# def func1(x):
#     print("before recursion", x)
    
#     if x > 10:
#         return
#     func1(x + 1)
#     print("after recursion", x)
# func1(1)

# def get_recursion_factorial(n):
#     if n == 1:
#         return 1
#     return n * get_recursion_factorial(n - 1)

# print(get_recursion_factorial(5))

# def get_loop_factorial(n):
#     sum_value = 1
#     while n > 1:
#         sum_value *= n
#         n -= 1
#     return sum_value
# print(get_loop_factorial(5))


# setup = """
# n = 1200
# def get_recursion_factorial():
#     global n
#     if n == 1:
#         return 1
#     return n * get_factorial(n - 1)

# def get_loop_factorial():
#     global n
#     sum_value = 1
#     while n > 1:
#         sum_value *= n
#         n -= 1
#     return sum_value
    
# def get_for_factorial():
#     global n
#     sume_value = 1
#     for i in range(1, n):
#         sume_value *= n
#     return sum_value
# """

# import timeit

# x = timeit.timeit(stmt="get_recursion_factorial", number=10000000, setup=setup)
# y = timeit.timeit(stmt="get_loop_factorial", number=10000000, setup=setup)
# z = timeit.timeit(stmt="get_for_factorial", number=10000000, setup=setup)

# print("recursion time : ", x)
# print("loop time: ", y)
# print("for time: ", z)
```
