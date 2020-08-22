<a.herf="https://mayadickson.github.io/Portfolio/">Home</a>


# Top 10 Disney movies at the box office
## Determines which 10 Disney movies earned the most at the box office
*This uses a Disney data compiled by Kelley Garrett, which containes 579 Disney movies with 6 features: movie title, release date, genre, MPAA rating, total gross, and inflation-adjusted gross.*

This is done by:
1. Importing pandas
    1. In order to read the csv file
2. Reading the Disney file into gross
3. Sorting the data based on the inflation adjusted gross column
    1. In descending order
4. Calling a head of 10 on the data to show the top 10 movies


```python
import pandas as pd
gross= pd.read_csv('disney_movies_total_gross.csv', parse_dates= ['release_date'])

inflation_adjusted_gross_desc= gross.sort_values(by='inflation_adjusted_gross', ascending=False)
inflation_adjusted_gross_desc.head(10)
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
      <th>movie_title</th>
      <th>release_date</th>
      <th>genre</th>
      <th>mpaa_rating</th>
      <th>total_gross</th>
      <th>inflation_adjusted_gross</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>Snow White and the Seven Dwarfs</td>
      <td>1937-12-21</td>
      <td>Musical</td>
      <td>G</td>
      <td>184925485</td>
      <td>5228953251</td>
    </tr>
    <tr>
      <th>1</th>
      <td>Pinocchio</td>
      <td>1940-02-09</td>
      <td>Adventure</td>
      <td>G</td>
      <td>84300000</td>
      <td>2188229052</td>
    </tr>
    <tr>
      <th>2</th>
      <td>Fantasia</td>
      <td>1940-11-13</td>
      <td>Musical</td>
      <td>G</td>
      <td>83320000</td>
      <td>2187090808</td>
    </tr>
    <tr>
      <th>8</th>
      <td>101 Dalmatians</td>
      <td>1961-01-25</td>
      <td>Comedy</td>
      <td>G</td>
      <td>153000000</td>
      <td>1362870985</td>
    </tr>
    <tr>
      <th>6</th>
      <td>Lady and the Tramp</td>
      <td>1955-06-22</td>
      <td>Drama</td>
      <td>G</td>
      <td>93600000</td>
      <td>1236035515</td>
    </tr>
    <tr>
      <th>3</th>
      <td>Song of the South</td>
      <td>1946-11-12</td>
      <td>Adventure</td>
      <td>G</td>
      <td>65000000</td>
      <td>1078510579</td>
    </tr>
    <tr>
      <th>564</th>
      <td>Star Wars Ep. VII: The Force Awakens</td>
      <td>2015-12-18</td>
      <td>Adventure</td>
      <td>PG-13</td>
      <td>936662225</td>
      <td>936662225</td>
    </tr>
    <tr>
      <th>4</th>
      <td>Cinderella</td>
      <td>1950-02-15</td>
      <td>Drama</td>
      <td>G</td>
      <td>85000000</td>
      <td>920608730</td>
    </tr>
    <tr>
      <th>13</th>
      <td>The Jungle Book</td>
      <td>1967-10-18</td>
      <td>Musical</td>
      <td>Not Rated</td>
      <td>141843000</td>
      <td>789612346</td>
    </tr>
    <tr>
      <th>179</th>
      <td>The Lion King</td>
      <td>1994-06-15</td>
      <td>Adventure</td>
      <td>G</td>
      <td>422780140</td>
      <td>761640898</td>
    </tr>
  </tbody>
</table>
</div>


