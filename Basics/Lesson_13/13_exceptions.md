# 13. exceptions

## Chapter 1
### 1. default exceptions
### 2. try/except
### 3. else/finally


```python
# # 1. default exception


# l1 = [1, 2, 3, 4]

# l1[10] # IndexError

# # x = 5 // 0 # ZeroDivisionError

# print(111)


# 2. try/except


# try:
#     l1 = [1, 2, 3, 4]

#     l1[10] # IndexError
#     x = 5 // 0 # ZeroDivisionError
# except:
#     print("IndexError!!!")

# print('next lines')

# try:
#     l1 = [1, 2, 3, 4]

# #     l1[10] # IndexError
#     x = 5 // 0 # ZeroDivisionError
# except IndexError as e:
#     print(str(e))
    
# except ZeroDivisionError as e:
#     print(str(e))
    

# try:
#     l1 = [1, 2, 3, 4]

#     l1[10] # IndexError
#     x = 5 // 0 # ZeroDivisionError
# except Exception as e:
#     print(str(e))

# print('next lines')

    
# def divide_number(number, divider): # try with if
#     x = number // divider
#     return x

# divide_number(10, 0)

# def divide_number(number, divider): # try with if
#     try:
#         x = number // divider
#     except ZeroDivisionError as e:
#         return str(e)
    
#     except TypeError as e:
#         print(str(e))
#         x = int(number) // int(divider)
#     return x

# print(divide_number(10, "2"))
    
# try:
#     5 // 0
#     users = []
#     users[5]
#     users + 7
# except (IndexError, ZeroDivisionError) as e:
#     print(e) # error message
# except TypeError as e:
#     print(e) # error message
```

## Chapter 2
### 1. else/finally
### 2. nested try/except


```python
# 3. else/finally


# l1 = [1, 2, 3, 4]
# l1[10] # error

# print('script finished')

# try:
#     l1 = [1, 2, 3, 4]
#     l1[10]
# except IndexError as e:
#     print('you have error')
#     print(str(e))
    
# print('script finished')


# try:
#     l1 = [1, 2, 3, 4]
#     l1[10]
# except IndexError as e:
#     print('you have error')
#     print(str(e))
# else :
#     print('if we have no exception')
# print('script finished')
    
    
# try:
#     l1 = [1, 2, 3, 4]
#     l1[10]
# except IndexError as e:
#     print('you have error')
#     print(str(e))
#     l1 = [1,2,3,4]
#     l1[10]
# finally:
#     print('in finally block')
# print('script finished')

# try:
#     numbers = [1, 2, 3, 4, 5]
#     raise IndexError # raised the error manually
# except IndexError:
#     print('got exception')

# x = 1
# assert x < 0, 'x must be negative'

# users = []
# assert users, 'user field is required'

# def show_users(users):
#     assert users, 'user field is required'
#     print(users)
    
# show_users(users)

# try:
#     l1 = [1,2,6]
#     l1.append(5)
#     try:
#         raise ZeroDivisionError()
#     except:
#         print('nested error')

#     print(55)

# except:
#     print('error here')
# else:
#     print('if we don\'t have exception')


# 2. nested try/except    

    
# def divide_number(number, divider): # try with if
#     try:
#         x = number // divider
#     except ZeroDivisionError as e:
#         return str(e)
    
#     except TypeError as e:
        
#         x = int(number) // int(divider) # ask students a question
#     return x

# print(divide_number(10, "abc"))



# def divide_number(number, divider): # try with if
#     try:
#         x = number // divider
#     except ZeroDivisionError as e:
#         return str(e)
    
#     except TypeError as e:
        
#         x = int(number) // int(divider) # ask students a question
#     return x

# print(divide_number(10, "abc"))


# catch error after call function
# def divide_number(number, divider): # try with if
#     x = number // divider
#     return x

# try:
#     print(divide_number(10, "12")) # ZeroDivisionError
#     print(divide_number(10, 0)) # TypeError
# except ZeroDivisionError as e:
#     print(str(e))
# except TypeError as e:
#     print(str(e))
```
