# EXNO-5-DS-DATA VISUALIZATION USING MATPLOT LIBRARY

# Aim:
  To Perform Data Visualization using matplot python library for the given datas.

# EXPLANATION:
Data visualization is the graphical representation of information and data. By using visual elements like charts, graphs, and maps, data visualization tools provide an accessible way to see and understand trends, outliers, and patterns in data.

# Algorithm:
STEP 1:Include the necessary Library.

STEP 2:Read the given Data.

STEP 3:Apply data visualization techniques to identify the patterns of the data.

STEP 4:Apply the various data visualization tools wherever necessary.

STEP 5:Include Necessary parameters in each functions.

# Coding and Output:

 ```python
import matplotlib.pyplot as plt
import numpy as np
import pandas as pd

x = [2018, 2019, 2020, 2021, 2022]
y = [15000, 20000, 25000, 30000 , 35000]
plt.plot(x, y, 'g*', linestyle='dashed', linewidth=2, markersize=12)
plt.xlabel('x-axis')
plt.xlabel('y-axis')
plt.title('2D Diagram')
plt.show()
```
<img width="571" height="453" alt="download" src="https://github.com/user-attachments/assets/add971e4-6657-4bac-a235-d4d63f5dea54" />

```python
plt.subplot(2,2,1)
plt.plot(x,y,'r--')
plt.subplot(2,2,2)
plt.plot(x,y,'g--')
plt.subplot(2,2,3)
plt.plot(x,y,'bo')
plt.subplot(2,2,4)
plt.plot(x,y,'go')
```
<img width="577" height="413" alt="download" src="https://github.com/user-attachments/assets/da2b1f56-7b60-470e-82f6-600fd04be09b" />

```python

x = np.arange(0, 4*np.pi, 0.1)
y = np.sin(x)
plt.title('sine waveform')
plt.plot(x, y)
plt.show()

```
<img width="568" height="433" alt="download" src="https://github.com/user-attachments/assets/d6b729a4-4922-4e9d-9ddf-a75f273f0924" />

```python

x = [2, 8, 10]
y = [11, 16, 9]
x1 = [3, 9, 11]
y1 = [6, 15, 7]
plt.bar(x, y, color='r')
plt.bar(x1, y1, color='g')
plt.title('Bar graph')
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.show()
```
<img width="563" height="453" alt="download" src="https://github.com/user-attachments/assets/748cd817-350b-4eff-a674-0f4ef2245b88" />

```python

x = [1, 2, 3]
y = [7, 3, 9]
plt.plot(x, y, color='g')
plt.title('line graph')
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.show()
```

<img width="554" height="453" alt="download" src="https://github.com/user-attachments/assets/1f756962-e1a1-4f02-bad8-5e317ed57996" />

```python
x1 = [1, 2, 3]
y1 = [2, 4, 1]
plt.plot(x1, y1, label='line1')
x2 = [1, 2, 3]
y2 = [4, 1, 3]
plt.plot(x2, y2, label='line2')
plt.title('multiline graph')
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.legend()
plt.show()
```
<img width="567" height="453" alt="download" src="https://github.com/user-attachments/assets/0dcd5c67-2b9d-49c3-bee3-0859cb387c8d" />


```python
x = [1, 2, 3, 4, 5, 6]
y = [2, 4, 1, 5, 2, 6]
plt.plot(x, y, color='green', linestyle='dashed', linewidth=3, marker='o', markerfacecolor='red', markersize=12, label='spices')
plt.ylim(1, 8)
plt.xlim(1, 8)
plt.title("Line graph")
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.legend()
plt.show()
```
<img width="558" height="453" alt="download" src="https://github.com/user-attachments/assets/89b97f6a-6fe6-4183-aa68-651397402e3e" />


```python
yield_apples = [0.895, 0.91, 0.919, 0.926, 0.929, 0.931]
plt.plot(yield_apples, linestyle='dashed', linewidth=3, marker='*', markersize=12, color='g')
plt.show()
```
<img width="565" height="413" alt="download" src="https://github.com/user-attachments/assets/95607425-4d6f-4f04-ba5d-9b5aed2c3f0f" />

```python

oranges = [2, 4, 6, 7, 8, 12, 45]
apples = [2, 4, 5, 6, 8, 23, 37]
years = [2019, 2020, 2021, 2022, 2023, 2024, 2025]
plt.plot(years, apples, marker='o')
plt.plot(years, oranges, marker='*')
plt.title('crop yields in kanto')
plt.xlabel('year')
plt.ylabel('yield (tons per hectare)')
plt.legend(['apples', 'oranges'])
plt.show()
```
<img width="563" height="453" alt="download" src="https://github.com/user-attachments/assets/ac515caa-feaf-42bc-9a4c-33f393c9c736" />

```python
oranges = [2, 4, 6, 7, 8, 12]
apples = [2, 4, 5, 6, 8, 23]
years = [2019, 2020, 2021, 2022, 2023, 2024]
plt.bar(oranges, apples)
plt.plot(years, apples, label='apples', marker='*')
plt.plot(years, oranges, label='oranges', marker='o')
plt.title('Fruit sales')
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.legend()
plt.show()
```
<img width="563" height="453" alt="download" src="https://github.com/user-attachments/assets/d6b220e3-34df-40f2-bbe7-f7968fee154c" />

```python
plt.figure(figsize=(12, 6))
plt.plot(years, oranges, marker='o', label='oranges')
plt.title("Yield of oranges (tons per hectare)")
plt.legend()
```
<img width="977" height="526" alt="download" src="https://github.com/user-attachments/assets/80e82ce0-5be2-45f0-a3a5-0d25322a1a39" />

```python
print("scatter plot is:")
x = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
y = [2, 4, 5, 7,6, 8, 9, 11, 12, 12]
plt.scatter(x, y, label='star', color='green', marker='*', s=30)
plt.title("my scatterplot!")
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.legend()
plt.show()
```
<img width="563" height="453" alt="download" src="https://github.com/user-attachments/assets/ef98b806-528c-44be-a1a3-18869d7a7145" />

```python
x=[1,2,3,4,5]
y1=[10,12,14,16,18]
y2=[5,7,9,11,13]
y3=[2,4,6,8,10]
plt.fill_between(x,y1,color='green',label='y1')
plt.fill_between(x,y2,color='blue',label='y2')
plt.fill_between(x,y3,color='red',label='y3')
plt.title("fill between is")
plt.legend()
plt.show()
```
<img width="556" height="433" alt="download" src="https://github.com/user-attachments/assets/e06de403-7691-430a-ba1f-fd12ed012792" />

```python

plt.stackplot(x,y1,y2,y3 , labels=['line1', 'line2','line3'])
plt.legend(loc='upper left')
plt.title("Stacked line chart")
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.show()
```
<img width="563" height="453" alt="download" src="https://github.com/user-attachments/assets/1eae9dc4-f4b2-484e-b519-3484de9054db" />

```python
from scipy.interpolate import make_interp_spline
x = np.array([1, 2, 3, 4, 5, 6, 7, 8, 9, 10])
y = np.array([2, 4, 5, 7, 8, 9, 10, 11, 12, 13])
spl = make_interp_spline(x, y)
x_smooth = np.linspace(x.min(), x.max(), 100)
y_smooth = spl(x_smooth)
plt.plot(x, y, 'o', label='data')
plt.plot(x_smooth, y_smooth, '-', label='spline')
plt.legend()
plt.show()
```
<img width="543" height="413" alt="download" src="https://github.com/user-attachments/assets/33a5b1b5-19b9-4d4a-a1e4-0967701c3837" />

```python

values = [5, 6, 7, 3, 2]
names = ['A', 'B', 'C', 'D', 'E']
plt.bar(names, values, color='green')
plt.show()
```
<img width="534" height="413" alt="download" src="https://github.com/user-attachments/assets/15a28cdd-cf81-41c5-a054-84c6273a3ab8" />

```python
ages = [2, 5, 70, 40, 45, 50, 43, 40, 44, 60, 7, 13, 57, 18, 90, 77, 32, 21, 20, 40]
range1 = (0, 100)
bins = 10
plt.hist(ages, bins, range1, color='green', histtype='bar', rwidth=0.8)
plt.xlabel('ages')
plt.ylabel('no.of people')
plt.title('my histogram')
plt.show()
```
<img width="554" height="453" alt="download" src="https://github.com/user-attachments/assets/595f6a7c-830c-4926-a8f6-601e629dd398" />

```python
x = [2, 1, 6, 2, 4, 8, 9, 4, 2, 4, 10, 6, 4, 5, 7, 7, 3, 2, 7, 5, 3, 5, 9, 2, 1]
plt.hist(x, bins=10, color='green', alpha=0.5)
plt.show()
```
<img width="534" height="413" alt="download" src="https://github.com/user-attachments/assets/19041ce5-9e92-4d67-9344-3a2ebfdef8bd" />


```python
np.random.seed(0)
data = np.random.normal(loc=0, scale=1, size=100)
data
```
<img width="577" height="323" alt="image" src="https://github.com/user-attachments/assets/e9984abb-4fc4-435c-886a-b7eb75bb45f6" />

```python

fig, ax = plt.subplots()
ax.boxplot(data)
ax.set_xlabel('x-axis')
ax.set_ylabel('y-axis')
ax.set_title('box plot')
```
<img width="565" height="453" alt="download" src="https://github.com/user-attachments/assets/7179bb45-7658-42c2-9ab4-883d2425d6b9" />

```python

activities=['eat' , 'sleep' , 'work' , 'play']
slices=[3,7,8,6]
colors=['r','y','g','b']
plt.pie(slices , labels=activities , colors=colors,startangle=90 , shadow = True , explode = (0,0,0.1,0) , radius = 1.2 , autopct="X1.1")
plt.legend()
plt.show
```
<img width="435" height="401" alt="download" src="https://github.com/user-attachments/assets/62786fbd-1712-417b-b721-114c220fd3f6" />

```python
labels='python','C+','ruby','java'
sizes=[215,130,245,210]
colors=['gold','yellowgreen','lightcoral','lightskyblue']
explode=(0,0.4,0,0.5)
plt.pie(sizes, explode=explode , colors=colors,labels=labels, autopct="%1.1f%%", shadow = True )
plt.axis('equal')
plt.show()
```
<img width="515" height="389" alt="download" src="https://github.com/user-attachments/assets/fb9c9cc9-a406-43e3-a06d-7551ed4677af" />


# Result:
Thus , the data visualization was peformed using matplot python library for the given datas successfully.
