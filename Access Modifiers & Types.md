Access specifiers and access modifiers in python programming are used to limit access of class variable and class methods outside of the class while implementing the concepts of inheritance.

Types:
1. Public access modifiers
2. Private
3. Protected

### PUBLIC
 All the variables and methods (member functions) in python are by default public. Any instance variable in a class followed by the ‘self’ keyword ie. self.var_name are public accessed.

	Unlike in C++ OR Java, where class attributes and methods are private by default.

![[Pasted image 20260302003309.png]]

### PRIVATE

Private members of a class are those members which can only be accessible inside the class.

In py, there is no strict concept of "private" modifiers only a convention. 
A variable or method should be considered private by prefixing its name with a double underscore (__). This is known as a "weak internal use indicator". This blocks general inheritance but can still be accessed through "[[name mangling]]".

![[Pasted image 20260302005513.png|396]]

### Protected

In OOPs, "protected" is used to describe a member of a class that is meant to accessed only by the class itself and its subclasses.
 In Python, the convention for indicating that a member is protected is to prefix its name with a single underscore (_). For example, if a class has a method called _my_method, it is indicating that the method should only be accessed by the class itself and its subclasses.

It's important to note that the single underscore is just a naming convention, and does not actually provide any protection or restrict access to the member.


![[Pasted image 20260302012040.png|366]]

