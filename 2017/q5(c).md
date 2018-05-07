## (c)(i)
```py
a = np.array([2,6,2,6])
b = np.array([8,4,9,4])

print(f1(a,b))
# [2,6,2,6] - [8,4,9,4] => [-6,-2,-7,2]
# abs([-6,-2,-7,2])     => [6,2,7,2]
# [6,2,7,2].sum()       => 17

print(f2(a,b))
# [2,6,2,6] - [8,4,9,4] => [-6,-2,-7,2]
# square([-6,-2,-7,2])  => [36,4,49,4]
# [36,4,49,4].sum()     => 93
# np.sqrt(93)           => 9.64

print(f3(a,b))
# np.dot([2,6,2,6],[8,4,9,4]) => 16 + 24 + 11 + 10 => 82
# TL; DD (Too long, didn't do)
```

## (c)(ii)
- f1 is Manhattan distance
- f2 is Minkowski distance (which is a generalization of Euclidean distance)
- f3 is Mahalanobis??

Note: Refer [DM-02.pdf](http://wble-sl.utar.edu.my/wble-sl/file.php/9981/DM.2018.01_DM-02.pdf)