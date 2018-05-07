## (i)
```py
import numpy as np
d = np.array([3,5,2,7,4,13,1,8,9,7,10,12]).reshape(3,-1) 
# means 3 rows, with number of element in each row automatically specified

# d is 
#   [
#       [3,5,2,7],
#       [4,13,1,8],
#       [9,7,10,12]
#   ]
```
Answer
```py
# Minimum value in the list
print(d.min()) # 1

# Index of maximum value
# The max is 13, which have index of 5
print(d.argmax()) # 5 


print(d.mean(axis=1)) # [(3+5+2+7)/4,(4+13+1+8)/4,(9,7,10,12)/4] = [4.25, 6.5, 6.25]

d.mean() # average of all numbers = 5.667

d.mean(axis=0) # [(3+4+9)/3,(5+13+7),(2,1,10),(7,8-1)]

# When axis is 0, means count average based on column

# When axis is 1, means count average based on rows

# When axis is -1, means based on its own shape



```


## (ii)
```py
print(d[d>5].size) # number of elements that is more than 5, which is 7

print(d[:,2]) # [2,1,10]

print(d.tranpose() * 2) 
# [[3,4,9],[5,13,7],[2,1,10],[7,8,12]] * 2
# [[6,8,18],[10,26,14],[4,2,20],[14,16,24]]
```