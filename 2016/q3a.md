## (i)
Tweleve dimensions.

## (ii) Cosine distance
Refer DM-02.
```
cosineSimilarityBetween a and b -> (a dot b)/((vectorLength a) * (vectorLength b))

vectorLength a:Number[] -> Number
  -> map square_ to a >> sum_ >> squareRoot_
```


## (iii) Hamming distance
```python
a    = (1,0,0,0,1,0,0,0,1,1,1,0)
b    = (0,0,1,1,1,0,0,0,0,0,0,0)
c    = (1,1,0,1,0,0,1,1,1,0,0,0)

# 0 means no diff, 1 means got diff
ham(a,b) => (1,0,1,1,0,0,0,0,1,1,1,0)

ham(a,c) => (0,1,0,1,1,0,1,1,0,1,1,0)
```
The `ham` with the least `1`s is has the least Hamming distance.

a is closer with b in Hamming distance since `ham(a,b)` has lesser `1`s then `ham(a,c)`.

## (iv) Manhattan distance
```py
manhattan(a,b) = sum(abs(diff(a,b)))

ab = abs(diff(a,b)) # (1,0,1,1,0,0,0,0,1,1,1,0)

ac = abs(diff(a,c)) # (0,1,0,1,1,0,1,1,0,1,1,0)

ab = sum(ab) # 6
ac = sum(ac) # 7
```
So, a is closer to b in terms of Hamming distance.
