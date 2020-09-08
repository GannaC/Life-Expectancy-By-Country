import codecademylib3_seaborn
import numpy as np
import pandas as pd
import matplotlib.pyplot as plt

data = pd.read_csv("country_data.csv")

#print(data.head())
life_expectancy = data['Life Expectancy']
# print(life_expectancy)
life_expectancy_quartiles = np.quantile(life_expectancy,[0.25, 0.5, 0.75])
# print(life_expectancy_quartiles)
# plt.hist(life_expectancy)
# plt.show()
gdp = data['GDP']
print(gdp)
median_gdp = np.quantile(gdp, [0.5])
#print(median_gdp)
low_gdp = [i for i in gdp if i <= median_gdp]
#for x in low_gdp:
#  print(x)
high_gdp = [i for i in gdp if i > median_gdp]
max = 0;
for x in high_gdp:
  if x > max:
    max = x
print ('biggest GDP: ',max)
plt.hist(data["Life Expectancy"], alpha = 0.5, label = "High GDP")
plt.show()
plt.hist(data["Life Expectancy"], alpha = 0.5, label = "Low GDP")
plt.legend()
plt.show()
print(data)

