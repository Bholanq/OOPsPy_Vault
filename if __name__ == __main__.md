`if __name__ = "__main__":` is used when we want to run the file only if it is the **main** program not when it is being imported.

Every python file has a built in module, `__name__` , if you run the file directly python set `__name__` to `__main__` , otherwise if we import the file as a module python will set the 
`__name__` variable to "filename"




For example:
## Case1
```
def greet():
    print("Hello!")
if __name__ == "__main__":
    greet()
```

suppose if the file name is file.py, then
if we run the file directly ie. python file.py 
then the output will be : Hello!

but if we import the file using 
`import file`
then the output will nothing.

## Case2 : if we don't put the function under the main condition

file.py :
```
def greet():
    print("Hello!")
greet()
```

then contradictory to the previous case `import file` will also output: Hello!


