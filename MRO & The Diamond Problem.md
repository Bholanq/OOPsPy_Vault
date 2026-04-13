
- Method Resolution Order 
**MRO = the order in which Python looks for a method in a class hierarchy.**

Python follows 3 main rules:
### 1. Child before parent

### 2. Left to right

### 3. No class appears twice
If two parent classes have the same method, Python must decide:

👉 “Which one should I execute?”

That decision is made using **MRO (C3 Linearization Algorithm)**

EG1. **Multiple Inheritance**

![[Pasted image 20260301220346.png|175]]

EG2. Diamond Problem 
      A
     / \
    B   C
     \ /
      D
      
Python checks in this order:
1. D
    
2. B
    
3. C
    
4. A
    
5. object
  


