Allows you to assign a value to a variable within an expression
# := 

```
numbers = [1,2,3,4,5]
while (n:= len(numbers))>0:
    print(numbers.pop())
n = len(numbers)
#OR
while n>0:
    print(numbers.pop())
    n = len(numbers)
```

Both the codes are the same