# 14. iterators, list comprehension, generators

## Chapter 1
### 1. iterators


```python
# 1. iterators


# numbers = [1, 2, 3]
# for i in numbers:
#     print(i)
    
# print(2 in numbers)

# f = open('file.txt')
# print(f.__next__())
# print(f.__next__())
# print(f.__next__())
# print(f.__next__())
# print(f.__next__())
# print(f.__next__()) # error StopIteration

# import collections
# isinstance([1, 2, 3], collections.Iterable)

# print(iter(f) is f) # True
# f.close()
# L = [1, 2, 3]
# print(iter(L) is L) # False
# print(L.__next__())

# I = iter(L) # allow call to __next__ method 
# print(I)
# print(I.__next__())
# print(I.__next__())

# some_dict = {"a":1, "b":2, "c":3}
# some_iter = iter(some_dict)
# next(some_iter) # ask question

# for key in D:
#     print(key, D[key])

# R = range(5)
# I = iter(R)
# next(I)
    
# lines = f.readlines()
# lines = [line.rstrip() for line in lines]
# lines = [line.rstrip() for line in open('file.txt')]
```

## Chapter 2
### 1. list comprehension
### 2. generators


```python
# 2. list comprehension

# result = []
# for x in 'spam':
#     result.append(x*2)
# print(result)

# print(result)

# result = [x * 2 for x in 'spam']
# print(result)

# [x for x in range(5) if x % 2 == 0]

# 3. generators

# def gensquares(N):
#     for i in range(N):
#         yield i ** 2
    
# G = gensquares(5)   
# next(G)
# for i in [gensquares(5)]:
#     print(i)

# L = [x ** 2 for x in range(4)]
# print(L)

# z = list(x ** 2 for x in range(4))

# (x ** 2 for x in range(4))

# G = (c * 4 for c in 'SPAM')

# def timesfour(S):
#     for c in S:
#         yield c * 4
        
# G = timesfour('spam')
# print(next(G))

# import sys
# old_L = [0, 1, 2, 3, 4, 5, 6]

# l = [n*2 for n in old_L] # List comprehension
# g = (n*2 for n in old_L)  # Generator expression

# print(type(l))  # 'list'
# print(type(g))  # 'generator'

# print(sys.getsizeof(old_L))  # 9024
# print(sys.getsizeof(l))  # 9024
# print(sys.getsizeof(g))  # 80

# z = {x * x for x in range(10)} # set
# print(type(z))
# res = set()
# for x in range(10):
#     res.add(x * x)
    
# {x: x * x for x in range(10)} # dict
```
