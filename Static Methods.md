Static methods are method that belong to the class rather than the instance of the class. They are defined using the  @staticmethod decorator and do not have access to the instance of the class(i.e self). 

Static methods are often used to create utility functions that don't need access to instance data.

![[Pasted image 20260308163836.png]]

In this example, the add method is a static method of the Math class. It takes two parameters a and b and returns their sum. The method can be called on the class itself, without the need to create an instance of the class.

We use static methods mainly when we want to ship methods along with the class.