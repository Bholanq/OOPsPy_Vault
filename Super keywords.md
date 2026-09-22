The super() keyword is Python is used to refer to the parent class. It is useful when a class inherits from multiple parent classes and you want to call a method from one of the parent classes.

When a child inherits from a parent class, it can override or extend the methods defined in the parent class. However, sometimes you might want to use the parents class's method in the child class. This is where the super keyword is handy.

`class parentclass:
`    def parent_method(self):`
`        print("this is a parent1 method")`
`class childclass(parentclass):`
`    def child_method(self):`
`        print("This is child1 method")`
`    def parent_method(self):`
`        return super().parent_method()`
`child1 = childclass()`
`child1.parent_method()`
OUTPUT:
`this is a parent1 method`


[[Method Overriding]]
[[Operator Overloading]]