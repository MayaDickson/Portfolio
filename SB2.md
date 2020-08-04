# Super Bowls highest and lowest combined scores

*This uses super bowl data compiled from Wikipedia.*

This is done by:
1. Importing pandas
    1. In order to read the csv file
2. Reading the super bowl file into super_bowls
3. Displaying the super bowl data that has
    1. Combined points greater than 70
    2. Combined points less than 70


```python
import pandas as pd
super_bowls = pd.read_csv('super_bowls.csv')

display(super_bowls[super_bowls['combined_pts'] > 70])
display(super_bowls[super_bowls['combined_pts'] < 25])
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>date</th>
      <th>super_bowl</th>
      <th>venue</th>
      <th>city</th>
      <th>state</th>
      <th>attendance</th>
      <th>team_winner</th>
      <th>winning_pts</th>
      <th>qb_winner_1</th>
      <th>qb_winner_2</th>
      <th>coach_winner</th>
      <th>team_loser</th>
      <th>losing_pts</th>
      <th>qb_loser_1</th>
      <th>qb_loser_2</th>
      <th>coach_loser</th>
      <th>combined_pts</th>
      <th>difference_pts</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>2018-02-04</td>
      <td>52</td>
      <td>U.S. Bank Stadium</td>
      <td>Minneapolis</td>
      <td>Minnesota</td>
      <td>67612</td>
      <td>Philadelphia Eagles</td>
      <td>41</td>
      <td>Nick Foles</td>
      <td>NaN</td>
      <td>Doug Pederson</td>
      <td>New England Patriots</td>
      <td>33</td>
      <td>Tom Brady</td>
      <td>NaN</td>
      <td>Bill Belichick</td>
      <td>74</td>
      <td>8</td>
    </tr>
    <tr>
      <th>23</th>
      <td>1995-01-29</td>
      <td>29</td>
      <td>Joe Robbie Stadium</td>
      <td>Miami Gardens</td>
      <td>Florida</td>
      <td>74107</td>
      <td>San Francisco 49ers</td>
      <td>49</td>
      <td>Steve Young</td>
      <td>NaN</td>
      <td>George Seifert</td>
      <td>San Diego Chargers</td>
      <td>26</td>
      <td>Stan Humphreys</td>
      <td>NaN</td>
      <td>Bobby Ross</td>
      <td>75</td>
      <td>23</td>
    </tr>
  </tbody>
</table>
</div>






<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>date</th>
      <th>super_bowl</th>
      <th>venue</th>
      <th>city</th>
      <th>state</th>
      <th>attendance</th>
      <th>team_winner</th>
      <th>winning_pts</th>
      <th>qb_winner_1</th>
      <th>qb_winner_2</th>
      <th>coach_winner</th>
      <th>team_loser</th>
      <th>losing_pts</th>
      <th>qb_loser_1</th>
      <th>qb_loser_2</th>
      <th>coach_loser</th>
      <th>combined_pts</th>
      <th>difference_pts</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>43</th>
      <td>1975-01-12</td>
      <td>9</td>
      <td>Tulane Stadium</td>
      <td>New Orleans</td>
      <td>Louisiana</td>
      <td>80997</td>
      <td>Pittsburgh Steelers</td>
      <td>16</td>
      <td>Terry Bradshaw</td>
      <td>NaN</td>
      <td>Chuck Noll</td>
      <td>Minnesota Vikings</td>
      <td>6</td>
      <td>Fran Tarkenton</td>
      <td>NaN</td>
      <td>Bud Grant</td>
      <td>22</td>
      <td>10</td>
    </tr>
    <tr>
      <th>45</th>
      <td>1973-01-14</td>
      <td>7</td>
      <td>Memorial Coliseum</td>
      <td>Los Angeles</td>
      <td>California</td>
      <td>90182</td>
      <td>Miami Dolphins</td>
      <td>14</td>
      <td>Bob Griese</td>
      <td>NaN</td>
      <td>Don Shula</td>
      <td>Washington Redskins</td>
      <td>7</td>
      <td>Bill Kilmer</td>
      <td>NaN</td>
      <td>George Allen</td>
      <td>21</td>
      <td>7</td>
    </tr>
    <tr>
      <th>49</th>
      <td>1969-01-12</td>
      <td>3</td>
      <td>Orange Bowl</td>
      <td>Miami</td>
      <td>Florida</td>
      <td>75389</td>
      <td>New York Jets</td>
      <td>16</td>
      <td>Joe Namath</td>
      <td>NaN</td>
      <td>Weeb Ewbank</td>
      <td>Baltimore Colts</td>
      <td>7</td>
      <td>Earl Morrall</td>
      <td>Johnny Unitas</td>
      <td>Don Shula</td>
      <td>23</td>
      <td>9</td>
    </tr>
  </tbody>
</table>
</div>




```python

```
