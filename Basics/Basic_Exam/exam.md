# Exam
```
Տեսական հարցեր
	1.	Կարճ պատմեք ձեր մասին, ինչով եք զբաղվել և հիմա ինչով եք զբաղվում:
	
	2.	Ինչու եք վորոշել զբաղվել ծրագրավորումով:
	
	3.	Ինչ data type-եր գիտեք և ինչ խմբերի կարող եք բաժանել:
	
		3.1 tuple-ի ու list-ի տարբերությունը:
			
		3.2 set-ի ու dict-ի տարբերությունը ու ձեր կարծիքով որն է ավելի արագ աշխատում և ինչու:
		
		3.3 Ինչ ընդհանուր գործիքներ կան iterator-ների համար:
		
		3.4 	x = [1, 2, 3, [4, 5, 6, [7, 8]]]]
				
				y = x[3].copy()
		
				y[3][0] = 25

				x[3][3][0]
				
		3.5		[
					[1,  2,  3,  4],
					[5,  6,  7,  8],
					[9,  10, 11, 12],
					[13, 14, 15, 16]
				]
				
				Ինչպես կարող ենք տպել թվերը անկյունագծով
				
		3.6	users_1 = ["Lilit", "Aren", "Janna", "Jarvis"]
				
				users_2 = ["Samvel", "Gohar", "Armen", "Luiza"]
				
				users = users_2 + users_1 # տարբերություն կլնի եթե փոխենք տեղերով
				
				users_with_slice = users_1[:2] + users_2[3:]
				
				users[0:15]
				
		3.7	numbers = [1, 4, 1, 5, 8, 4] ոնց կարանք սարքենք unique
	
	4.	if else
		
		4.1 if 5 > 7 and 0 == False
		
		4.2 if 5 > 7 or 0 == False
		
	5	for while
		
		5.1	Ինչպես կարող ենք ստանալ	անվերջ cycle for-ի միջոցով:
		
		5.2 Ինչ կստանանք հետեվյալ արտահայտություց
		
			users = ["Lilit", "Aren", "Janna", "Jarvis"]
			
			for user in users:
				users.pop()
			print(users)
		
		5.3 for with else
		
		
	6.	functions
		
		6.1 Ինչ առավելություններ են տալիս մեզ function-ները:
		
		6.2	Ինչ տեսակի parameter-ներ կան և ինչ հերթականությամբ է պետք դրանք հայտարարել
		
		6.3	def login():		
				email = 'test@gmail.com'
				
				def local_func(name):
					return 'name is ' + name + ', email is ' + email
				
				return local_func
			x = login()
			
			x('Vardan')
			
	7.	module
		
		7.1 package-ի և module-ի տարբերությունը
		
		7.2	Ինչպես package-ից import անել միայն մեկ module-ը
		
		7.3 Ինչպես import անել package-ի բոլոր մոդուլները
		
	8. 	exceptions
		
		8.1 Որ դեպքերում կարող են պետք գալ exception-ները:
		
		8.2 Երբ է աշխատում finally բլոկը:
		
		8.3 Երբ է աշխատում else բլոկը:
		
		8.4 Ինչպես կարող ենք առաջացնել արհեստական exception-ներ:
		
	9.	generators
		
		9.1 Ինչով են տարբերվում list comprehension-ը generator-ից
		
		9.2 Ինչպես կարող ենք function-ը դարձնել generator:
		
		9.3 Ինչ առավելություն ունի generator-ը սովորական for-ի նկատմամբ:

		def generator():
			yield 1
			yield 2
			yield 3
		
		x = generator()
		print(next(x))
		print(next(x))
		
	10. functional programing
	
		10.1 Ինչ առավելություններ ունի functional programing-ը
		
		10.2 Ինչ function-ներ գիտեք functional programing-ի համար
		
	11.	decorators
		
		11.1 Ինչ է decorator-ը և ինչ առավելություններ է տալիս:
		
		11.2 Ինչ տարբերություն կա տրված decorator-ների մեյ:

				def decorator_1(func):
					def wrapper():
						print('code from decorator')
						func()
					return wrapper
					
				def decorator_1(func):
					def wrapper():
						func()
						print('code from decorator')
					return wrapper
		
		11.3 Ինչպես կարող ենք օգտագոծել decorator առանց @-ի
		
	12. regexp
	
		12.1 Ինչ է regex-ը և օգտագործվում է արդյոք միայն python-ում 
		
		12.2 Նշեք regex-ի ինչ operator-ներ գիտեք

			
	13. pep
		
		13.1 Ինչ է pep-ը:
		
		13.2 Նշեք pep-ի կանոններից մի քանիսը
		
Խնդիրներ
	
	1.	reverse list:
	
	2.	deep copy - manually:
		[1, 2, 3, [4, 5, [6, 7]]]
	
	3	Գնտել և տպել list-ով 0-100 բոլոր պարզ թվերը:
	
	4. fibonacci
		Գտեք 7-րդ fibonacci-ի թիվը:
		
	5.	Գնտել minimum-ը
		[12, 78, 2, 3, 6, 100, 28]
		
	
	
```
