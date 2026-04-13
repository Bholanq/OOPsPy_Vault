### 1. `reverse()` (method)

- Works **only on lists**
- **Modifies the original list in place**
- Returns **`None`**

nums = [1, 2, 3]  
nums.reverse()  
print(nums)   # [3, 2, 1]
If you try:
x = nums.reverse()  
print(x)   # None
### 2. `reversed()` (function)

- Works on **any iterable** (list, tuple, string, etc.)
- Does **NOT modify original**
- Returns an **iterator**
nums = [1, 2, 3]  
rev = reversed(nums)  
print(list(rev))  # [3, 2, 1]  
print(nums)       # [1, 2, 3] (unchanged)