# Homework №11

```
	1.	Գրել get_secure_data function որը կվերադարձնի passwords.txt file-ի
		data-ն հետեվյալ format-ով 
		[
			{'Vardan' : '123456789'} # user name and passwords
			{'Armen' : '987654321'}
		]
		
	2.	Գրել decorator get_secure_data function-ի համար որը որպես parameter
		կստանա "user" կամ "admin":
		
		user - ստանալու դեպքում վերադարձնել error
		admin - ստանալու դեպքում վերադարձնել get_secure_data-ն
		
	3.	Գրել ևվս մեկ decorator get_secure_data function-ի համար
		որը error-ի դեպքում(եթե parameter = "user") error-ը և datetime-ը
		կգրի log.txt file-ում:
		
		# որոշել decorator-ների անունները և հերթականությունը
		@decorator2
		@decorator1("user")
		get_secure_data():
			...
			
	4.	Ստեղծել decorators.py file, decorator1 և decorator2-ի կոդը տեղափոխել այնտեղ,
		import անել և օգտագործել main.py file-ում որտեղ գրված է get_secure_data function-ը:
```


### Research
```
	1.	class-ով decorator-ի պարամետր:
```


### Links

```
Կարող եք օգտվել հետեվյալ link-երից:
https://www.geeksforgeeks.org/decorators-with-parameters-in-python/
https://www.geeksforgeeks.org/class-as-decorator-in-python/
https://realpython.com/primer-on-python-decorators/
```
