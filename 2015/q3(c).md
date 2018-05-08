## (i)
The purpose of this code snippet is to identify the relationship between each feature for each class.  
In this case:  
    - `Xs` is column 1, which is the `sepal width`.  
    - `Ys` is column 2, which is the `petal length`.

There are 3 classes, where:  
    - 0 means `setosa`  
    - 1 means `versicolor`  
    - 2 means `virginica`

So, where are trying to identify the relationship between `sepal width` and `petal length` for each classes.

## (ii)
This is part is hard to explain, so I'll just explain part of the code.  
The symbol `=>` means return.  
For example, if `[9,8,7][0]` will return `9`,  I will write it as `[9,8,7][0] => 9`

Note that `=>` is not a valid symbol in Python.  It's just for explanation purpose.
```py
len(markers) => 3
range(3)     => [0,1,2]
Xs[:]        => Xs  # Dr. Tay tries to trick people with this
Ys[:]        => Ys 

t==0         => [False,False,False,False,False,False,True]

t==1         => [True,False,True,False,True,False,False]

t==2         => [False,True,False,True,False,True,False]


Xs[[False,False,False,False,False,False,True]] => [3.4]

Xs[[True,False,True,False,True,False,False]] => [3, 2.4, 3]


```

### Final output

![image](https://user-images.githubusercontent.com/23183656/39741895-1e5a2c64-52ce-11e8-9d8b-a320cb492897.png)





