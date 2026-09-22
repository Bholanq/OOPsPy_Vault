Magic methods aka ''dunder'' methods, from the double underscores surrounding their names, are tools that allow you to customize the behavior of your class.

`class emp:
`    name = "Harry"  `
`    def __len__(self):`
`        i = 0`
`        for c in self.name:`
`            i=i+1`
        `return` i
`e = emp()`
`print(e.name)`
`print(len(e))`

Eg. In the above case we define the dunder function 
`__len__` in the class, which determines what the output should be when len(obj) is called for an obj of that class. Similarly:

| Method        | Purpose                                   |
| ------------- | ----------------------------------------- |
| `__init__`    | Constructor (runs when object is created) |
| `__str__`     | Defines what `print(object)` shows        |
| `__repr__`    | Official string representation            |
| `__len__`     | Defines `len(object)`                     |
| `__add__`     | Defines `+` operation                     |
| `__eq__`      | Defines `==` comparison                   |
| `__getitem__` | Enables indexing `obj[i]`                 |
| `__iter__`    | Makes object iterable                     |

