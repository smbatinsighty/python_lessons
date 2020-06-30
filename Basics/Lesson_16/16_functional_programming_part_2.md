# 16. functional programming part 2

## Chapter 1
### 1. compose
### 2. decorator


```python
### 1. compose

# def double(x):
#     return 2 * x

# def inc(x):
#     return x + 1

# # print(inc(double(3)))

# def compose(f1, f2):
#     return lambda x: f1(f2(x))

# z = compose(inc, double)
# y = compose(double, inc)
# print(z(3))
# print(y(3))

### 2. decorator

# def auth(func): # add @decorator
#     def wrapper():
#         print("auth package started")
#         func()
#         print("auth package finished")
#     return wrapper


# def login():
#     print(f'user logged in')


# def register():
#     print(f'user registered')
        
# # login = auth(login)
# login()
# # # register = auth(register)
# register()


# def auth(func):
#     def wrapp(name):
#         print("auth package started")
#         func(name)
#         print("auth package finished")
#     return wrapp

# @auth
# def login(name):
#     print(f'user {name} logged in')

# @auth
# def register(name):
#     print(f'user {name} registered')
        
# # login = auth(login)
# login("Vardan")
# register("Vardan")


# def auth(func):
#     def wrapp(name):
#         print("auth package started")
#         func(name)
#         print("auth package finished")
    
#     return wrapp

# def second_auth(func):
#     def wrapp(name):
#         print("second decorator started")
#         func(name)
#         print("second decorator finished")
#     return wrapp

# @auth
# @second_auth
# def login(name):
#     print(f'user {name} logged in')

# @auth
# @second_auth
# def register(name):
#     print(f'user {name} registered')
    
# # login = auth(login)
# login("Vardan")
# # register = auth(register)
# register("Vardan")    

# def auth_wrapp(arg1, arg2):
#     def auth(func):
#         def wrapp(name):
#             print("auth package ", arg1)
#             func(name)
#             print("auth package ", arg2)
#         return wrapp
#     return auth

# @auth_wrapp("started", "finished")
# def login(name):
#     print(f'user {name} logged in')

# @auth_wrapp("started", "finished")
# def register(name):
#     print(f'user {name} registered')
    
# login("Vardan")
# register("Vardan")
# login = auth_wrapp("started", "finished")(login)
# login("Vardan")
```
