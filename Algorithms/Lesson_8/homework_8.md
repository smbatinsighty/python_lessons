# Homework №8
```
    
    1.  FIFO VS LIFO (նշել նաև որ datastructure֊ներն են ռեալիզացնում)։
   
    
    2.  Օգտագործելով list ռեալիզացրեք queue որի միջոցով կկարողանաք հերթականույամբ կանչել տրված 3 function-ները անդադար։
        Առաջադրանքը կատարել research-ի 1֊ին կետը անելուց հետո։
   
    def task1():
        print("function 1 started")
        sleep(2)
        print("function 1 finshed")
    def task2():
        print("function 2 started")
        sleep(2)
        print("function 2 finshed")
    def task3():
        print("function 3 started")
        sleep(2)
        print("function 3 finshed")
    >>> function 1 started
    >>> function 1 finshed
    >>> function 2 started
    >>> function 2 finshed
    >>> function 3 started
    >>> function 3 finshed
    >>> function 1 started
    >>> function 1 finshed
    >>> function 2 started
    >>> ...
    >>> ...
```
### Research
```
    1.   sleep from time
    2.   deque from collections
    3.   Ինչ է := operator֊ը python-ում և որ version-ից սկսած է հասանելի
```