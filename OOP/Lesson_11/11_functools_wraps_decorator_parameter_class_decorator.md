# 11. method decorator, decorator for class

### 1. functools.wraps


```python
# from functools import wraps

# def my_decorator(func):
#     @wraps(func)
#     def wrap():
        
#         """
# my wrapper documentation
#         """
#         print('before my func')
#         func()
#     return wrap
    
# @my_decorator
# def my_func():
#     """
# my func documentation
#     """
#     print('from my func')

# print(my_func.__name__)
# print(my_func.__doc__)
# my_func()
```

### 2. decorator with parameters


```python
# def add_type(return_type):
#     def float_and_return(function):
#         def wrapper(*args, **kwargs):
#             args = [float(arg) for arg in args]
#             result = function(*args, **kwargs)
#             if return_type == "float":
#                 result = float(result)
#             elif return_type == "int":
#                 result = int(result)
#             return result

#         return wrapper
#     return float_and_return

# @add_type("float")
# def mean(first, second, *rest):
#     numbers = (first, second) + rest
#     return sum(numbers) / len(numbers)

# mean(1, 2, 3, "9")
# float_and_return = add_type("int")
# mean = float_and_return()
# mean(1, 2, 3, "4")
```

### 3. class decorator


```python
# class MyDecorator:
#     def __init__(self, func):
#         print('decorator init')
#         self.func = func
        
#     def __call__(self):
#         print('decorator call method')
#         self.func()
        
        
# @MyDecorator
# def my_func():
#    print('from my func')
    
# my_func()
```


```python
# class MyDecorator:
    
#     def __init__(self, func):
#         print('decorator init')
#         self.func = func
        
#     def __call__(self):
#         print('decorator call method')
#         self.func()

# def my_func():
#     print('from my func') 

# myfunc = MyDecorator(my_func) 
# myfunc()
```
