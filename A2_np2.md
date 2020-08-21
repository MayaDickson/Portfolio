# 2D NumPy array
## Creating the 2D NumPy array
*Uses a list of reaction time (rt) and error (err) values from a Flanker-Simon study. The rt values are given in milliseconds and the err values are displayed as booleans. When err= True this means that the trail was an error.*

This is done by:

1. Importing numpy
    1. In order to convert the lists (rt, err) into a 2D array
2. Call the functioon np.array( ) on the lists
3. Print the array


```python
rt = [0.551714007, 0.344355373, 0.282130643, 0.388339099, 0.741976576, 0.426807824, 0.589848489, 0.341542697, 0.287110004, 0.322289797, 0.379822366, 0.336714422, 0.333802666, 0.293643588, 0.386914908, 0.282874789, 0.383207132, 0.416732649, 0.329448009, 0.554469006, 0.523510978, 0.341133708, 0.508971072, 0.389857974, 0.404175466]

err = [False, False, True, False, False, False, False, False, False, False, False, False, False, True, False, False, True, True, False, False, False, False, False, False, False]
```


```python
import numpy as np

dat= np.array([rt, err])
print(dat)
```

    [[0.55171401 0.34435537 0.28213064 0.3883391  0.74197658 0.42680782
      0.58984849 0.3415427  0.28711    0.3222898  0.37982237 0.33671442
      0.33380267 0.29364359 0.38691491 0.28287479 0.38320713 0.41673265
      0.32944801 0.55446901 0.52351098 0.34113371 0.50897107 0.38985797
      0.40417547]
     [0.         0.         1.         0.         0.         0.
      0.         0.         0.         0.         0.         0.
      0.         1.         0.         0.         1.         1.
      0.         0.         0.         0.         0.         0.
      0.        ]]


## Calculating the error rate
*Using the error list from above, an error rate can be produced and printed out*

This is done by:
1. Counting the number of errors produced and dividing it by the total number of trials
    1. Calling the method .count( ) will give the number of errors produced
    2. Calling the function len( ) will give the total number of trials
2. Multiplying by 100
    1. This converts it into a percentage
3. Print the error rate


```python
err_rate= (err.count(True)/len(err)) *100
print(err_rate)
```

    16.0

