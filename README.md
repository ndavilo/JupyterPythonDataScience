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

#!/usr/bin/env python
# coding: utf-8

# In[1]:


import pandas as pd
import numpy as np
import seaborn as sns
import matplotlib.pyplot as plt


# In[2]:


data = pd.read_csv(r"EKITI-STATE-ELECTION-RESULT.csv")


# In[3]:


data.head()


# In[5]:


data.columns


# In[6]:


data


# In[15]:


sns.relplot(x="APC votes", y="Ekiti LGA's ", data=data)


# In[17]:


sns.relplot(x="PDP votes", y="Ekiti LGA's ", data=data)


# In[16]:


sns.relplot(x="SDP votes", y="Ekiti LGA's ", data=data)


# In[21]:


sns.relplot(x="S/N", y="APC votes", hue="Ekiti LGA's ", data=data)


# In[22]:


sns.relplot(x="S/N", y="PDP votes", hue="Ekiti LGA's ", data=data)


# In[23]:


sns.relplot(x="S/N", y="SDP votes", hue="Ekiti LGA's ", data=data)


# In[24]:


sns.pairplot(data)


# In[31]:


sns.relplot(x="S/N", y="APC votes", kind="line", data=data)


# In[32]:


sns.relplot(x="S/N", y="PDP votes", kind="line", data=data)


# In[35]:


sns.relplot(x="S/N", y="SDP votes", kind="line", data=data)


# In[38]:


sns.catplot(x="S/N", y="SDP votes", data=data)


# In[ ]:




