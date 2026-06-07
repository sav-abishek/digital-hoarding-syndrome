# Load basic libraries
	import pandas as pd
	import matplotlib.pyplot as plt
	import seaborn as sns
	import numpy as np

# Access the data
	data_url = 'https://archive.ics.uci.edu/ml/machine-learning- databases/wine-quality/winequality red.csv'
	data = pd.read_csv(data_url, sep=";")


## 1. Check data samples

![[Pasted image 20230212164427.png]]

## 2. Understand the significance of all features

![[Pasted image 20230212164629.png]]

## 3. Data statistics

![[Pasted image 20230212164648.png]]

### Plotting histogram
![[Pasted image 20230212164824.png]]

## 4. Create Test Set

 - Avoid data snooping bias (a form of statistical bias manipulating data or analysis to artificially get statistically significant results)
 - Scikit learn provides a few functions to create test sets:
		**Random Sampling** - randomly selects k% points in the test set.
		**Stratified Sampling** - samples test examples in such a way that they are
		representative of the overall distribution, avoids bias that may arise due to
		random sampling
--------------------------------------------------------------

