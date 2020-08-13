# 12. meta classes

### 1. meta classes


```python
# print(type([]))
# print(type(type))
# print(list.__class__)
# print(list().__class__)

# class User:
#     pass

# User = type("User", )

# user = User()
# print(user.__class__)
 
# class Meta(type):
#     def __new__(meta, class_name, supers, class_dict):
#         print("meta", meta) # Meta class
#         print(class_name) # User - child class name
#         print(supers) # parent classner@
#         print(class_dict) # User class attibutes
#         return type.__new__(meta, class_name, supers, class_dict)
    

    

# class SpaceMan:
#     pass

# class User(SpaceMan, metaclass = Meta):
#     name = 'Jarvis'
    
    
# jarvis = User()
```


```python
# ## __init__

# class Meta(type):
#     def __new__(meta, class_name, supers, class_dict):
#         # print(meta) # Meta class
#         # print(class_name) # User - child class name
#         # print(supers) # parent classner@
#         # print(class_dict) # User class attibutes
#         return type.__new__(meta, class_name, supers, class_dict)
        
#     def __init__(self, class_name, supers, class_dict):
#         print('Meta Init method')
#         print(Class) # User class
#         print(class_name) # User - child class name
#         print(supers) # parent classner@
#         print(class_dict) # User class attibutes
        


# class SpaceMan:
#     pass

# class User(SpaceMan, metaclass = Meta):
#     name = 'Jarvis'
    
# print("----------User--------", User)
# jarvis = User()
```


```python
# def MetaFunc(class_name, supers, class_dict):
#     print(class_name) # User - child class name
#     print(supers) # parent classner@
#     print(class_dict) # User class attibutes
#     return 1

# class SpaceMan:
#     pass

# class User(SpaceMan, metaclass = MetaFunc):
#     name = 'Jarvis'

# print(User)
# jarvis = User()
# print(jarvis)
```


```python
# class SuperMeta(type):
#     def __call__(meta, classname, supers, classdict):
#         print('SuperMeta call method: ')
#         return type.__call__(meta, classname, supers, classdict)
        


# class Meta(type, metaclass = SuperMeta):
    
#     def __new__(meta, class_name, supers, class_dict):
#         print('Meta New method')
#         # print(meta) # Meta class
#         # print(class_name) # User - child class name
#         # print(supers) # parent classner@
#         # print(class_dict) # User class attibutes
#         return type.__new__(meta, class_name, supers, class_dict)
        
#     def __init__(Class, class_name, supers, class_dict):
#         print('Meta Init method')

        
# class SpaceMan:
#     pass

# class User(SpaceMan, metaclass = Meta):
#     name = 'Jarvis'

# jarvis = User()
```

    SuperMeta call method: 
    <class '__main__.Meta'> User
    Meta New method
    Meta Init method



```python
# class User:
#     def __init__(self):
#         print("init")
        
#     def __new__(self):
#         print(11)
#         return self

# User = type("Vazgen", (), {"asd": "basd"})
# User.status = "haramiq"
# print("User", User.status)
# user = User()
```
