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
gross= pd.read_csv('datasets/disney_movies_total_gross.csv', parse_dates= ['release_date'])

inflation_adjusted_gross_desc= gross.sort_values(by='inflation_adjusted_gross', ascending=False)
inflation_adjusted_gross_desc.head(10)
```
