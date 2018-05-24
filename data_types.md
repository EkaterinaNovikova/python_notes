# Data types
## String
Make all letters capitalized
```my_str.upper()```

Make first letter in a string capitalized
```my_str.capitalize()```

```my_str.replace('replaced_string', 'replacing_string')```

#### Count letters in a string
```string.count('a')```


## List
`[, , ,]` <- any data type including strings, floats, booleans, etc.

`list.append(value)` add value

`index()` get the index of the first element of a list that matches its input

`count()` get the number of times an element appears in a list

`append()` add an element to the list it is called on

`remove()` remove the first element of a list that matches the input

`reverse()` reverse the order of the elements in the list it is called on

## Dictionary
`{key : value}` 
`{'A' : 1, 'B' : 3}`

#### Take value by key
```
dict = `{'A' : 1, 'B' : 3}`
dict['A']
>>> 1
```

#### Create dictionary
```
my_dict = {key1 : value, key2 : value2}
```

#### Return keys
```
dict.keys()
```

#### Delete key-value
```
del(dict[key])
```
#### Add key-value to dict
```dict['new_key'] = new_value```

#### Dictionary may contain dictionary
```dict = {key1 : {key11: value11, key12 : value12}, key2: {key21 : value21, key22 : value22}}```
take elements:
```dict[key1][key12]```

#### Loop for
```
for key.value in dict.items():
```
## Numpy array
#### Create numpy array from a list
``` 
import numpy as np
my_nparr = np.array(my_list)
```
#### Transpose
```
y = np.array([[7, 8, 9], 
              [11, 12, 13]])
np.transpose(y)

>>> array([[ 7, 11],
       [ 8, 12],
       [ 9, 13]])
```
#### Element-wise calculations (element by element)
```my_array * 3```

#### Comparing of arrays
```
np.logical_and(array1 > 21, array1 < 22)
array1[np.logical_and(array1>21, array1 < 22)]
```

#### Subsetting of 2d arrays
```
regular list of lists
x = [["a", "b"], ["c", "d"]]
[x[0][0], x[1][0]]

import numpy as np
np_x = np.array(x)
np_x[:,0]
```
#### Print out the 50th row of np_array
```print(np_array[49, :])```

#### Loop for
```
for val in np.nditer(array):
```
#### Median and mean
```np.mean(x)
np.median(x)
```

## Pandas data type
Parse dates:
```
df = pd.read_csv(filename, parse_dates = ['Date']
```
Parse and use dates as indexes:
```
df = pd.read_csv(filename, index_col = 'Date', parse_dates = True)
```
Convert list of dates into a datetime object:
```
time_format = '%Y-%m-%d %H:%M'
my_datetimes = pd.to_datetime(date_list, format=time_format)  
```
To get a DataFrame as a numpy array
```df.array()```
