# 7. If else elif, while

## Chapter 1
### 1. bool
### 2. if
### 3. else
### 4. elif
### 5. short if
### 6. switch case


```python
# 1. bool

# print(bool(""))

# print(bool(0))

# print(bool("0"))

# print(bool(-1))

# print(bool([]))

# print(bool([""]))

# print(bool([[]]))

# is

# 2. if

# print("before if")
# x = 7
# if True:
#     print("print in if")
    
# print("after if")

# 3. else

# x = 1
# if x > 1:
#     print("x meca 1-ic")
    
# else:
#     print("x poqra 1-ic")
    
    
# print("code finished")

# age = input("how old are you? ")
# if age.isnumeric():
#     age = int(age)
#     if age > 18:
#         print("qachalanum gnum es banak!")
#     else:
#         print("visilit es linum")
# else:
#     if age == "chem uzum grem":
#         print("jandam gres")
#     print("please write your age not string")
# print("code finished")
        
        
# age = int(input("how old are you? "))

# if age > 18:
#     print("qachalanum gnum es banak!")
# else:
#     if age > 15:
#         print("visilit es linum")
#     else:
#         print("vabshe visilit es linum")
#         print("< 18-ic")
# print("code finished")

# 4. elif
    
# age = int(input("how old are you? "))
# if age >= 18:
#     print("age > 18-ic")
# elif age >= 15:
#     print("age > 15")
# else:
#     print("age < 15")
# print("code finished")

# 5. short if
# age = int(input("how old are you? "))
# message = 'welcome' if age >= 18 else "go away"
# print(message)

# message = input("please rite message") or "there is not message"
# print(message)


# 6. switch case

# x = input()
# unit_to_multiplier = {
#     'mm': 10**-3,
#     'cm': 10**-2,
#     'dm': 10**-1,
#     'm': 1,
#     'km': 10**3
# }.get(x, 0)

# print(unit_to_multiplier)
```

## Chapter 2
### 1. while
### 2. break, continue


```python
# 1. while

# x = 0
# while x < 10:
#     x = x + 1
#     print(x)
    
# print("loop finished x =", x)


# while True:
#     print("aaaaa")

# 2. break, continue

# break

# x = 0
# while x < 10:
#     x = x + 1
#     if x == 7:
#         break
        
#     print(x)
    
# print("loop finished x =", x)

# continue

# x = 0
# while x < 10:
#     x = x + 1
#     if x == 7:
#         continue
        
#     print(x)
    
# print("loop finished x =", x)
```
