# The PhoneBook Example

Let	us	imagine	that	we	want	to	build	a simple PhoneBook	application,	capable	of	storing	a	set	
of	contacts for	each	registered	person.	A	person	has	a	name	and	each	contact	is	represented	
by	a name	and	a	phone	number.

## Describing	the	Domain

The	 domain	 model	 of	 the	 PhoneBook	 application consists only	 of	three entities:	 ```PhoneBook```,
```Person``` and	```Contact```.	The	```PhoneBook``` entity	represents	the	class	that	knows	all	registered	people.	
Each	person	maintains	his/her	own	set	of	contacts.

## Describing	entities using	the	DML

Using	the	DML,	we	could	textually	describe	the	domain	model	of	our	PhoneBook	application	
through	the following	DML	code:

```
1. class PhoneBook;
2.
3. class Person	{
4. 		String	name;
5. }
6.
7. class Contact {
8. String name;
9. String phoneNumber;
10. }
```

There	are	other	business	rules	that	should	be	implemented.	For	instance,	consider	that	it	
should	be	possible	to	remove	a	```Contact``` given	its	name, and	getting all	```Contact``` instances	
whose	 name	 contains	 a	 given	 substring. These	 would	 correspond	 to	 the	implementation	 of	
methods	in	the	Person class	with	the	desired	functionality.
