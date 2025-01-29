
**Step 1:** Setting up libraries and installing packages

A **library** is a collection of code that you can use in your programs, while a **package** is a folder that contains libraries or other packages, organized for easy use.

To install a library, I'll use the following format:
```python
 import <library name> as <shortname>
```
I use a *short name* since it is easier to refer to the package to access functions and also to refer to subpackages within the library.

import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns
import folium

**Step 2**

Let’s access our data. I will be using the NYC OpenData Motor Vehicle Collisions - Crashes dataset. According to NYC Open Data, "each row represents a crash event. The Motor Vehicle Collisions data tables contain information from all police reported motor vehicle collisions in NYC."

database link: [https://drive.google.com/file/d/12XPI1kNaRlBQpoTAlvuaXYpUUohfGCYT/view?usp=drive_link](url)

```
from google.colab import drive
drive.mount('/content/drive')
```

**TODO: Read the data using pandas read_csv function**

```
data = pd.read_csv("/content/drive/MyDrive/Motor_Vehicle_Collisions_-_Crashes_20241229.csv")
```

**Step 3:** Let's see what the data looks like. I can use the `head` function which returns the first 5 rows of the dataset.

**TODO: Print the first 5 rows of the data using head function of pandas**
```
data.head(5)
```

**TODO: Describe the data using the describe function of pandas**
```
desc_stats = data.describe()
desc_stats
```
