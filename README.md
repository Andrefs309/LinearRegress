# LinearRegress


## IMPORTAÇÕES
import numpy as np
import matplotlib.pyplot as plt
import math
import pandas as pd
%matplotlib inline


## LER OS DADOS DE UM FICHEIRO CSV 
## Valores de X e Y - DUAS PRIMEIRAS COLUNAS
data = pd.read_csv(r"C:\Users\USER\Documents\data.csv")
X = data.iloc[:, 0]
Y = data.iloc[:, 1]

## Taxa de Aprendizagem - TERCEIRA COLUNAS
alpha = data.iloc[0, 2]


## Função da recta --> Y = b + mx
## Definir valores iniciais para "b" e "m"
b = data.iloc[0, 3]
m = data.iloc[0, 4]
