# Data Structures & Algorithms №1  
### Introduction
<br/>

<img src="image_1.png" width="1000" style="margin:auto"/>

## 1. Intro

* About Course and Sources

* What Are Algorithms

* Why We Should Learn Algorithms

## 2. Algorithm Visualization

* Diagram

*  Pseudocode

* Code

### 2.1. Diagram

* Linear algorithms

<img src="diagram_1-Linear.svg" width="135" style="margin:auto"/>

* Conditional Logic Algorithm

<img src="diagram_1-Conditional.svg" width="300" style="margin:auto"/>

* Cyclic Algorithms

<img src="diagram_1-Cyclic.svg" width="390" style="margin:auto"/>

### 2.2. Pseudocode 
num = input("write number")  
while num > 0  
    sum += num % 10  
    num // 10  
output sum
### 2.3. Code


```python
num = int(input("write number "))
sum_digits = 0
while num > 0:
    sum_digits += num % 10
    num //= 10
print(sum_digits)
```

## 3. Binary Search

<img src="binary_search-Page-1.svg" width="700" style="margin:auto"/>

<img src="binary_search-Page-2.svg" width="700" style="margin:auto"/>

<img src="binary_search-Page-3.svg" width="700" style="margin:auto"/>

<img src="binary_search-Page-4.svg" width="700" style="margin:auto"/>


```python
# Write code for binary search with students
```


```python
def binary_search(list, item):
    low = 0
    high = len(list)-1
    while low <= high :
        mid = (low + high) // 2
        guess = list[mid]
        if guess == item :
            return mid
        if guess > item:
            high = mid - 1
        else:
            low = mid + 1
    return None
my_list = [1, 3, 5, 7, 9]
x = binary_search(my_list, 9)

print(x)
```
