# 7. while part 2, for

## Chapter 1
### 1. While with list
### 2. While with dict


```python
# 1. While with list

# users = ["Gohar", "Aren", "Lilit", "Armen", "Luiza", "Samvel", "Janna"]
# x = 0
# while x < 6:
#     x += 1 # ask question to students
#     print(users[x])
    
# while users:
#     print(users)
#     users.pop()

# 2. While with dict

# new_users = []
# while users:
#     new_users.append(users.pop())
#     print(new_users)

# users = {"firstname": "Gohar", "age": "17", "mobile": "sensrov", "profession": "Python Developer"}
# user_keys = list(users.keys())
# while user_keys:
#     key = user_keys.pop()
#     print(key, "=", users[key])

# users = {"firstname": "Smbat", "age": "23", "mobile": "terev Nokia", "profession": "jarvis"}

# user_items = list(users.items())
# x = len(user_items)
# while x:
#     x -= 1
#     print("key = ", user_items[x][0], end=" ")
#     print("value = " ,user_items[x][1])
```

## Chapter 1
### 1. for, isinstance
### 2. range


```python
# 1. for, isinstance
# users = ["Gohar", "Aren", "Lilit", "Armen", "Luiza", "Samvel", "Janna"]

# for user in users:
#     print(user)

# users = ["Gohar", "Aren", "Lilit", "Armen", "Luiza", "Samvel", "Janna", ["Hovhannes", "Smbat"]]

# for user in users:
#     if isinstance(user, list):
#         for tutor in user:
#             print("tutor", tutor)
#     else:       
#         print("user", user)

# dict
        
# users = {"firstname": "Gohar", "age": "17", "mobile": "sensrov", "profession": "Python Developer"}

# for user in users:
#     print(user) # ask question to students

# for key, value in users.items():
#     print("key = ", key)
#     print("value = ", value)

# 2. range

# for x in range(10):
#     print(x)

# for x in range(10,100):
#     print(x)
    
# for x in range(10,100,5):
#     print(x)
    
# x = range(0, 20)
# print(type(x))
# print(list(x))
```

## Chapter 1
### 1. Short for


```python
# l1 = [1,2,3,4]
# l2 = [number for number in l1]
# print(l2)

# l1 = [1,2,3,4]
# l2 = [number * 2 for number in l1]
# print(l2)

# l1 = [1,2,3,4]        
# l2 = [number * 2 for number in l1 if number > 2]
# print(l2)

# users = ("Gohar", "Aren", "Lilit", "Armen", "Luiza", "Samvel", "Janna")
# new_users = ["my name is " + user for user in users ]
# print(new_users)
```
