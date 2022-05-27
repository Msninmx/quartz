---
title: "Basic Data Analysis in Python"
disableToc: true
---
### Basic Data Analysis in Python
```
import pandas as pd
import numpy as np
```

The two most important libraries in data analysis are Pandas and NumPy. Pandas allows us to read and manipulate different datasets, while NumPy lets us perform specific operations with these.

These libraries are imported using aliases, this is best practice.
#### Pandas
```
df = pd.read("file")
```

Here we read from a specific file and save it as a dataframe. `df` is used by convention.

```
df.head()
```

`head()` is used to show the first few rows and columns of the dataframe.

```
df.corr()
```

`corr()` prints a table that shows us the relationship between the different regressors. It's important that each one of these independent variables are con related between each other.
