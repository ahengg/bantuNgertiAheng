# The Look ECommerce Data Analysis

<p align="center">
  <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRAeydWteMBCJeaC4TLf3P7AMzhMbVef49HkA&s" alt="Logo" />
</p>

Ini adalah Jupyter notebook dari data Analysis
--
### Table Of Contets
- [Introduction](#introduction)
- [Pertanyaan](#Visualisasi Bisnis)
--
## isualisasi Bisnis
### 1-where-are-the-most-male-customers-located-display-with-a-bar-chart-per-country
```Python
import pandas as pd
import matplotlib.pyplot as plt

# Example data loading and processing (replace with actual data processing)
data = pd.read_csv('data.csv')
male_customers = data[data['gender'] == 'Male']
country_counts = male_customers['country'].value_counts()

# Plotting
plt.figure(figsize=(10, 6))
country_counts.plot(kind='bar')
plt.title('Number of Male Customers by Country')
plt.xlabel('Country')
plt.ylabel('Number of Male Customers')
plt.show()
```
