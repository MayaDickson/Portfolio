# Creating and Manipulating a NumPy array
## Converting a list to a NumPy array
*Takes a list of reaction times (rt) and makes it into a NumPy array. These rt values are given in seconds from a Flanker-Simon study.*

This is done by:

1. Importing numpy
    1. In order to convert the list into an array
2. Calling the function np.array( ) on the list
3. Printing the array


```python
rt = [0.551714007, 0.344355373, 0.282130643, 0.388339099, 0.741976576, 0.426807824, 0.589848489, 0.341542697, 0.287110004, 0.322289797, 0.379822366, 0.336714422, 0.333802666, 0.293643588, 0.386914908, 0.282874789, 0.383207132, 0.416732649, 0.329448009, 0.554469006, 0.523510978, 0.341133708, 0.508971072, 0.389857974, 0.404175466]
```


```python
import numpy as np

np_rt= np.array(rt)
print(np_rt)
```

    [0.55171401 0.34435537 0.28213064 0.3883391  0.74197658 0.42680782
     0.58984849 0.3415427  0.28711    0.3222898  0.37982237 0.33671442
     0.33380267 0.29364359 0.38691491 0.28287479 0.38320713 0.41673265
     0.32944801 0.55446901 0.52351098 0.34113371 0.50897107 0.38985797
     0.40417547]


## Manipulating the NumPy array
*The NumPy array above is manipulated in order to convert the rt values into milliseconds.*

This is done by:

1. Multiplying the array by 1000
    2. This converts the values from seconds to milliseconds
2. Printing the converted array


```python
np_rt_ms= np_rt*1000
print(np_rt_ms)
```

    [551.714007 344.355373 282.130643 388.339099 741.976576 426.807824
     589.848489 341.542697 287.110004 322.289797 379.822366 336.714422
     333.802666 293.643588 386.914908 282.874789 383.207132 416.732649
     329.448009 554.469006 523.510978 341.133708 508.971072 389.857974
     404.175466]

