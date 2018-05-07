## (i)
```
total = sum [95, 97, 100, 93, 4, 10, 2, 2, 2, 3, 4, 2, 12]
```

## (ii)
```
accuracy = (all trues)/total
```

## (iii)
```
error_rate = (all not trues)/total
```

### (iv)
The model is a little confused on how to differentiate between A and D, this is because:
- there are 12 D predicted as A
- and there are 10 A predicted as D

Even though all E are correctly predicted as E (high accuracy), however there are a lot of other non-E are also predicted as E, thus the number of False-Positive for E is high, so we say that the model is not precised enough at predicting an input as E(low precision).