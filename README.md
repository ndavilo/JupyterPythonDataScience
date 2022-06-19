# JupyterPythonDataScience
Python Data Science note
Libraries to import:

import pandas as pd
import numpy as np
import seaborn as sns
import matplotlib.pyplot as plt

data = pd.read_csv(r"file/location/filename.csv")
data.head()
data.discribe()
data.columns
sns.relplot(x='column name", y="another column name", data=data) #this is to plot the relationship between two columns
