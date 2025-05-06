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
NAME: MOHAN S
REG.NO: 212223240094
```
```python
import pandas as pd
import numpy as np
import seaborn as sns
import matplotlib.pyplot as plt
```
```python
x = [1, 2, 3, 4, 5]
y = [3, 6, 2, 7, 1]
```
```python
plt.plot(x,y,label='line1')
```
![Screenshot 2025-05-06 105707](https://github.com/user-attachments/assets/363a67cd-ca95-4647-acd0-ea774f00427d)

```python
x1 = [1,2,3]
y1 = [2,4,1]
x2 = [1,2,3]
y2 = [4,1,3]
```
```python
plt.plot(x1,y1,label='line1')
plt.plot(x2,y2,label='line2')
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('Two lines on same graph!')
plt.legend()
plt.show()
```
![Screenshot 2025-05-06 105831](https://github.com/user-attachments/assets/bbb4ce93-3b92-43e4-97f2-dcd2465849e1)

```python
import matplotlib.pyplot as plt
x=[1,2,3,4,5,6]
y=[2,4,1,5,2,6]
plt.plot(x,y,color='green',linestyle='dashed',linewidth=3,marker='o',markerfacecolor='blue',markersize=12)
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('Some cool customizations!')
plt.show()
```
![Screenshot 2025-05-06 105906](https://github.com/user-attachments/assets/6611b6d5-fbac-401f-99dd-a9c4b30e949a)

```python
yield_apples=[0.895,0.91,0.919,0.926,0.929,0.931]
plt.plot(yield_apples)
```
![Screenshot 2025-05-06 105942](https://github.com/user-attachments/assets/60d017d6-7072-4b7a-896d-331b54507e08)

```python
years=[2010,2011,2012,2013,2014,2015]
yield_apples=[0.895,0.91,0.919,0.926,0.929,0.931]
plt.plot(years,yield_apples)
```
![Screenshot 2025-05-06 110015](https://github.com/user-attachments/assets/0129e910-d31a-4adf-8942-1b4361d0dfa4)

```python
years=range(2000,2012)
apples=[0.895,0.91,0.919,0.926,0.929,0.931,0.934,0.936,0.937,0.9375,0.9372,0.939]
oranges=[0.926,0.941,0.930,0.923,0.918,0.908,0.907,0.904,0.901,0.898,0.9,0.896, ]
plt.plot(years, apples)
plt.plot(years, oranges)
plt.xlabel('Year')
plt.ylabel('Yield (tons per hectare)')
plt.title('Crop Yields in Kanto')
plt.legend(['Apples','Oranges']);
```
![Screenshot 2025-05-06 110101](https://github.com/user-attachments/assets/a1da5a6e-8812-47f4-9a29-fa374d516999)

```python
plt.figure(figsize=(12,6))
plt.plot(years,oranges,marker='o')
plt.title("Yield of Oranges (tons per hectare)");
```
![Screenshot 2025-05-06 110139](https://github.com/user-attachments/assets/a536517f-7ffb-4c03-8a02-ea9b74a6178d)

```python
import matplotlib.pyplot as plt
import numpy as np
import pandas as pd
x=np.arange(0,10)
y=np.arange(11,21)
x
```
![Screenshot 2025-05-06 110226](https://github.com/user-attachments/assets/1734c78c-fc43-49e1-97e6-35d98d59068e)

```python
y
```
![Screenshot 2025-05-06 110257](https://github.com/user-attachments/assets/d079f517-cd65-4527-9ccc-035046e084ab)

```python
plt.scatter(x,y,c='r')
plt.xlabel('X-axis')
plt.ylabel('Y-axis')
plt.title('Graph in 2D')
plt.savefig('Test.png')
```
![Screenshot 2025-05-06 110332](https://github.com/user-attachments/assets/d2d54bfb-4415-449a-ace6-9084e6503264)

```python
y=x*x
y
```
![Screenshot 2025-05-06 110403](https://github.com/user-attachments/assets/0be2ea38-4c58-47be-8242-00c767dc9d00)

```python
plt.plot(x,y,'g*',linestyle='dashed',linewidth=2,markersize=12)
plt.xlabel('X axis')
plt.ylabel('Y axis')
plt.title('2d Diagram')
plt.legend(['y-values']);
```
![Screenshot 2025-05-06 110444](https://github.com/user-attachments/assets/38f4c34a-7d2d-4cfb-823f-c5834beed478)

```python
x=np.arange(0,4*np.pi,0.1)
y=np.sin(x)
plt.title("sine wave form")
plt.plot(x,y)
plt.show()
```
![Screenshot 2025-05-06 110517](https://github.com/user-attachments/assets/e84db645-63a9-4514-b383-b4d642a7639b)

```python
import matplotlib.pyplot as plt
import numpy as np
x=[1,2,3,4,5]
y1=[10,12,14,16,18]
y2=[5,7,9,11,13]
y3=[2,4,6,8,10]
plt.fill_between(x,y1,color='blue')
plt.fill_between(x,y2,color='green')
```
![Screenshot 2025-05-06 110552](https://github.com/user-attachments/assets/aa268310-478c-4f8d-9328-b086b9617579)

```python
import matplotlib.pyplot as plt
import numpy as np
x=[1,2,3,4,5]
y1=[10,12,14,16,18]
y2=[5,7,9,11,13]
y3=[2,4,6,8,10]
plt.fill_between(x,y1,color='blue')
plt.fill_between(x,y2,color='green')
plt.plot(x,y1,color='red')
plt.plot(x,y2,color='black')
plt.legend(['y1','y2'])
plt.show()
```
![Screenshot 2025-05-06 110621](https://github.com/user-attachments/assets/2f37b451-57fc-4c23-b720-3d2fc1b81f41)

```python
import matplotlib.pyplot as plt
height=[10,24,36,40,5]
names=['one','two','three','four','five']
c1=['red','green']
c2=['b','g']
plt.bar(names,height,width=0.8,color=c1)
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('My bar chart!')
plt.show()
```
![Screenshot 2025-05-06 110657](https://github.com/user-attachments/assets/ec324b27-3b75-43f5-b127-6279da57ca8d)

```python
x=[2,8,10]
y=[11,16,9]
x2=[3,9,11]
y2=[6,15,7]
plt.bar(x,y,color='r')
plt.bar(x2,y2,color='g')
plt.title('Bar graph')
plt.ylabel('Y axis')
plt.xlabel('X axis')
plt.show()
```
![Screenshot 2025-05-06 110733](https://github.com/user-attachments/assets/6ea85e57-d376-4e75-8cc0-062100ae907f)

```python
import matplotlib.pyplot as plt
ages=[2,5,70,40,30,45,50,45,43,40,44,60,7,13,57,18,90,77,32,21,20,40]
range=(0,100)
bins=10
plt.hist(ages,bins,range,color='green',histtype='bar',rwidth=0.8)
plt.xlabel('age')
plt.ylabel('No. of people')
plt.title('My histogram')
plt.show()
```
![Screenshot 2025-05-06 110812](https://github.com/user-attachments/assets/89bc1ece-2286-437c-9c57-70a16a3a0ed3)

```python
import matplotlib.pyplot as plt
import numpy as np
np.random.seed(0)
data=np.random.normal(loc=0,scale=1,size=100)
data
```
![Screenshot 2025-05-06 110843](https://github.com/user-attachments/assets/f00bcb90-ff0f-43cd-b66b-21493d7904e4)

```python
fig,ax=plt.subplots()
ax.boxplot(data)
ax.set_xlabel('Data')
ax.set_ylabel('Values')
ax.set_title('Box Plot')
```
![Screenshot 2025-05-06 110914](https://github.com/user-attachments/assets/7213e2b3-63a8-47a0-b08c-626ed6747e7f)

```python
labels='Python','C++','Ruby','Java'
sizes=[215,130,245,210]
colors=['gold','yellowgreen','lightcoral','lightskyblue']
explode=(0,0.4,0,0.5)
plt.pie(sizes,explode=explode,labels=labels,colors=colors,autopct='%1.1f%%',shadow=True)
plt.axis('equal')
plt.show()
```
![Screenshot 2025-05-06 110944](https://github.com/user-attachments/assets/559b87f4-5ed6-496f-9b8b-1ec0ff212987)

```python
activities=['eat','sleep','work','play']
slices=[3,7,8,6]
colors=['r','y','g','b']
plt.pie(slices,labels=activities,colors=colors,startangle=90,shadow=True,explode=(0,0,0.1,0),radius=1.2,autopct='%1.1f%%')
plt.legend()
```
![Screenshot 2025-05-06 111021](https://github.com/user-attachments/assets/e587237d-ca9e-4949-aa9f-dc4a47150217)



# Result:
Thus the data visualization using matplot python library for the given datas are performed.
