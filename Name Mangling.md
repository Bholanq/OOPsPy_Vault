Name mangling is Python is a technique used to protect class-private and superclass - private attributes from accidently being overwritten by subclasses.

![[Pasted image 20260302011119.png]]

In the example above, the attribute _nonmangled_attribute is marked as nonmangled by convention, but can still be accessed from outside the class. The attribute __mangled_attribute is private and its name is "mangled" to _MyClass__mangled_attribute, so it can't be accessed directly from outside the class, but you can access it by calling _MyClass__mangled_attribute