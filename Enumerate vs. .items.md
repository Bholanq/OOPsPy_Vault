enumerate is use to iterate over any iterable object along with its index and keys.

```
list = [1,2,3]
for ind,key in enumerate(list):
	print(ind,key)

Output: 
0 1
1 2
2 3
```

**.items() , .keys() , .values()** are methods associated with the dictionary class:
.items for both key and values
.keys - just for keys 
.values - just for values

```
for index, (key, value) in enumerate(my_dict.items()):
    print(index, key, value)
0 a 1
1 b 2
2 c 3
```
