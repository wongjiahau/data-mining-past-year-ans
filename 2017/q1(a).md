## (i)
```py
# Questions
a = [2,4,6,8,10]
b = (2,4,6,8,10)
c = {2:"TWO",4:"FOUR",6:"SIX",8:"EIGHT",10:"TEN"}
```
```py
# Answers
print(a[2])    # 6
print(b[2:])   # (6,8,10)
print(c[2])    # "TWO"
```

## (ii)
```python
b[2] = 3  # Error, 'tuple' object does not support assignment

a[10] = 6 # Index out of range

c[10] = 5 # No error
```
```py
# Finally, c will look like this
{2:"TWO",4:"FOUR",6:"SIX",8:"EIGHT",10:5}
```
