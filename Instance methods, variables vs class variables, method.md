![[Pasted image 20260308164905.png|305]]
In python `emp1.showdetails()` is the same as 
`employee.showdetails(emp1)` , always taking in 1 argument. 
`emp1 can considered as 'self' here`

In Python, variables can be defined at the class level or at the instance level.

**Class variables** are defined at the class level and are shared among all instances of the class. They are defined outside of any method and are usually used to store information that is common to all instances of the class.

**Instance variables** are defined at the instance level and are unique to each instance of the class. They are defined inside the `__init__` method and are usually used to store information that is specific to each instance of the class.

eg

```
class students:
	def __init__(self,name,age):
	self.name = name
	self.age = age
	
s1 = students(alice,92)
```
Here name and age are instance variables as they're unique and defined for each instance.


Class variables can only be access and modified at the instance level.

## Class methods
![[Pasted image 20260308180751.png|278]]
The first parameter of the Class method is always `cls`

Here` cls` can be replaced with any variable, it just represents the class itself. Like how `self` represents the instance of the class.

Adding the decorator @classmethod 
will make it change, class variable itself.

![[Pasted image 20260308181508.png|472]]

Notice how employee.company is now tesla after adding the @classmethod 
A class variable can altered at the instance level or be changed at the class level using a class method along with `cls` - refers to the class

[[Class methods as alt constructors]]