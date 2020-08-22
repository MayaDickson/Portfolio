<a href="https://mayadickson.github.io/Portfolio/">Home</a>


# Descriptive Statistics
## Code 1
*This code determines the mean reaction time (RT) for the first 25 trails, in a Flanker-Simon study.*

This is done by:

1. Using the .loc indexer on the Pandas DataFrame and assigning it to dat_rt
    1. Slicing the rows from 0-24
    2. Selecting the RT columns values
2. Calling the method .mean( ) on dat_rt

```python
dat_rt= dat.loc[0:24,'rt']
dat_rt.mean()
```

``` python
405.6557296799999
```

## Code 2
*This code determines the mean reaction time (RT) for the congruent flankers in the Flanker-Simon study. It also rounds the mean RT to the nearest thousandths place.*

This is done by:
1. Using the .loc indexer on the DataFrame and assigning it to dat_congruent
    1. Stating that you only want the rows with congruent flankers
    2. Selecting the RT columns values
2. Calling the function round( ) and the method .mean( ) on dat_congruent
    1. Stating that you want to round to the thousandths place (3)

``` python
dat_congruent= dat.loc[dat['flankers']== 'congruent', 'rt']
round(dat_congruent.mean(), 3)
```

``` python
416.068
```

## Code 3
*This code determines the mean reaction time (RT) for the incongruent flankers in the Flanker-Simon study. It also prints out text that makes it clear that the computed mean RT belongs to the incongruent flankers.*

This is done by:
1. Using the .loc indexer on the DataFrame and assigning it to dat_incongruent
    1. Stating that you only want the rows with incongruent flankers
    2. Selecting the RT columns values
2. Adding text to print with the mean RT of dat_incongruent
    1. Calling print( )
        1. Inside " " add the desired text you want to add
        2. Add (+) the function str( )
            1. Applying the method .mean( ) to dat_incongruent

``` python
dat_incongruent= dat.loc[dat['flankers']== 'incongruent', 'rt']
print("Mean RT for incongruent flankers = " + str(dat_incongruent.mean()))
```

``` python
Mean RT for incongruent flankers = 439.9507526916668
```

<a href="https://mayadickson.github.io/Portfolio/A2_stat1.html">Back to Top</a>
