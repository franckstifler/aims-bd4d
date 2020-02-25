# Summary of day 2
## 1. Creating an api key on [openweathermap.org](https://openweathermap.org)
## 2. Python for Data Science
### 2.1 Essential data Science libraries in python
*Pandas*

Pandas has two main data structures: Series, DataFrames.

*Some Pandas function*
```python
import pandas as pd

# Set the name of the CSV file
data_file = '../data/power-outages.csv'

# Read data into dataframe
# dataframe is the pandas object for handling tabular data
df = pd.read_csv(data_file)

df.head(10) # Lists the first 10 elements

df.tail(6) # List the last 6 elements.

df.columns # List the columns of the file

df.describe() # Displays infos like avg, min, max of the data
```

### 2.2 Communicating with APIs
Make use of the `requests` package from Python.
```python
import requests
url_endpoint = "endpoint_to_access"
req = requests.get(url_endpoint)
response = req.json() # To get the json response of the api
print(response)
```

### 2.3 String formating in Python 3
```python
name = "Dunstan"
age = 60
name_and_age = "My name is {} and I am {}".format(name, age)
print(name_and_age)
# Output: My name is Dunstan and I am 60
```

### 2.2 data generation in python
### 2.3 case study: satelite image manipulation
