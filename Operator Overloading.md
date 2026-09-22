Operator Overloading is a feature in python that allows developers to redefine the behavior of mathematical and comparison operators for custom data types.

In the code below,
1. `__Str__` - determines what is actually printed when print() function is called on a class
2. `__add__` - determines what will happen when we use the "+" operator for objects of the specific class 
3. `x` - refers to the other class object except the self.
4. For for reference visit - https://docs.python.org/3/library/stdtypes.html

```
class vector:
    def __init__(self,i,j,k):
        self.i = i
        self.j = j
        self.k = k
    def __str__(self):
        return f"{self.i}i + {self.j}j + {self.k}k"
    def __add__(self,x):
        return vector(self.i + x.i, self.j+x.j, self.k+x.k)
v1 = vector(3,4,5)
print(v1)
v2 = vector(1,2,4)
print(v2)
print(v1+v2)
print(type(v1+v2))
```
Output:

![[Pasted image 20260322021324.png|318]]

