# Cypher
SIH 2k24


import pandas as pd
import numpy as np
from math import cos,sin,pi
import matplotlib as mpl
import matplotlib.pyplot as plt

d=pd.read_csv("RS_Session_260_AU_2323_C_to_D.csv")

d


from matplotlib import pyplot as plt
import seaborn as sns
d.groupby('Zone').size().plot(kind='barh', color=sns.palettes.mpl_palette('Dark2'))
plt.gca().spines[['top', 'right',]].set_visible(False)

x=d['Zone']
y=d['DRUG SEIZED']

plt.plot(x,y,'x')

e=pd.read_csv("RS_Session_260_AU_2308_A_to_B.csv")

e

y=e['Type of Drug']
x=e['2023']

plt.plot(x,y,'x')

f=pd.read_csv("RS_Session_260_AU_2323_C_to_D.csv")

f

y=f['Quantity of Drugs/Contraband ']
x=f['Zone']

plt.plot(x,y,'x')
