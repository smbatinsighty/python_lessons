# 5. Dictionary, and, or, not

## Chapter 1
### 1. Dictionary introduction
### 2. Dictionary is mutable


```python
#1. Dictionary introduction


# Example with contacts

# contacts = [["Vazgen", "098-46-56-76"], ["Gago", "099-35-23-23"]]
# "Gago" in contacts[0]
# "Gago" in contacts[1]
# print(contacts[1][0], contacts[1][1], sep=": ")

# x = dict()
# print(x)
# y = {}
# print(y)

# contacts = {"Vazgen": "098-46-56-76"}
# print(contacts)
# print(contacts['Vazgen'])

# x = dict(name = "Jarvis", age = 36, country = "USA")

# contacts["Gago"] = "099-35-23-23" 
# contacts["Gago"] = "099-11-11-11" # key unique
# contacts["space x"] = "fly"

# print(contacts["Vardan"])

# print(contacts.get("Vardan", "chka"))

# print(contacts) # the dictionary has no indexes


# 2. Dictionary is mutable


# x = {"name" : "jorj"}
# y = x
# x["name"] = 'valod'

# print(y)

# users_tests = [
#     ["Lilit", "Aren", "Janna", "Samvel (Sam)", "Gohar", "Armen", "Luiza"],
#     [[1, 2, 3, 4, 5, 6, 7], [8, 9, 10, 11, 12, 12, 14], [15, 16, 17, 18, 19, 20, 21]]
# ]

# users_tests = {
#     "Lilit": {"test_1": 1, "test_2": 8, "test_3": 15},
#     "Aren": {"test_1": 2, "test_2": 9, "test_3": 16}
# }

# print(users_tests["Lilit"])
# print(users_tests["Lilit"]['test_1'])

# users_tests["Janna"]["test_1"] = 3 # error

# users_tests["Janna"] = {"test_1": 3} # or
# users_tests["Janna"] = {}
# users_tests["Janna"]["test_1"] = 3
# print(users_tests)
```

    Lilit


## Chapter 2
### 1. Dictionary methods


```python
# users = {"firstName": "Vazgen", "lastName": "Gevorgyan", "phoneNumber": "0000"}

# users.clear() # remove all dict

# print(users.get("phoneNumber"))

# users.pop("firstName") # remove by key and return value

# print(users.keys()) # return dict keys in list

# print(users.values()) # return dict values in list

# print(users.items()) # return key, value in list with tuple

# dict1 = {1: 1, 2:4}
# dict2 = {3: 9, 4: 16}
# dict1.update(dict2) # add dict1 to dict2
# print(dict1)

# print(users)
```

## Chapter 3
### 1. And or not


```python
# 1. And or not

# 5 < 10 or 100 < 70 True or False
# 5 < 10 and 100 < 70 True and False
# 5 < 10 or not 100 < 70 True or not False

# users = {"firstName": "Vazgen", "lastName": "Gevorgyan"}
# "phoneNumber" not in users
# "firstName" not in users
# "firstName" in users or "phoneNumber" in users
```
