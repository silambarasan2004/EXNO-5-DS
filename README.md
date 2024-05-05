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

```
import matplotlib.pyplot as plt
x1=[1,2,3]
y1=[2,4,1]
plt.plot(x1,y1,label='line1')
x2=[1,2,3]
y2=[4,1,3]
plt.plot(x2,y2,label='line2')
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('Two lines on same graph!')
plt.legend()
plt.show()
```

![image](https://github.com/silambarasan2004/EXNO-5-DS/assets/119559917/6535605a-7c38-46e9-9db0-f350b3e50ef6)


```
import matplotlib.pyplot as plt
x=[1,2,3,4,5,6]
y=[2,4,1,5,2,6]
plt.plot(x,y,color='green',linestyle='dashed',linewidth=3,marker='o',markerfacecolor='blue',markersize=12)
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('Some cool customizations!')
plt.show()
```

![image](https://github.com/silambarasan2004/EXNO-5-DS/assets/119559917/4002dcd3-c5ae-4eee-9199-038afc7e9ec1)


```
yield_apples=[0.895,0.91,0.919,0.926,0.929,0.931]
plt.plot(yield_apples)
```

![image](https://github.com/silambarasan2004/EXNO-5-DS/assets/119559917/7b2a0680-2bac-4511-bfbd-c25ab919b3ff)


```
years=[2010,2011,2012,2013,2014,2015]
yield_apples=[0.895,0.91,0.919,0.926,0.929,0.931]
plt.plot(years,yield_apples)
```

![image](https://github.com/silambarasan2004/EXNO-5-DS/assets/119559917/227e2742-c1cf-4034-acdd-af6f0b3e531c)


```
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

![image](https://github.com/silambarasan2004/EXNO-5-DS/assets/119559917/bfc266d8-2483-4d65-86a6-94060e67bb8e)


```
plt.figure(figsize=(12,6))
plt.plot(years,oranges,marker='o')
plt.title("Yield of Oranges (tons per hectare)");
```

![image](https://github.com/silambarasan2004/EXNO-5-DS/assets/119559917/7d8ea26c-7fac-4fd3-bc86-dce81511c91f)


```
import matplotlib.pyplot as plt
import numpy as np
import pandas as pd
x=np.arange(0,10)
y=np.arange(11,21)
x

```
![image](https://github.com/silambarasan2004/EXNO-5-DS/assets/119559917/eea1a83f-48e9-4499-a5ea-4af6614b9300)
```
y
```
![image](https://github.com/silambarasan2004/EXNO-5-DS/assets/119559917/eb2265fc-cdd1-4d9d-8abd-63a3047416e5)
```
plt.scatter(x,y,c='r')
plt.xlabel('X-axis')
plt.ylabel('Y-axis')
plt.title('Graph in 2D')
plt.savefig('Test.png')
```
![image](https://github.com/silambarasan2004/EXNO-5-DS/assets/119559917/beb5b5c1-d6db-4a34-ab77-109e7cb82b78)
```
y=x*x
y
```
![image](https://github.com/silambarasan2004/EXNO-5-DS/assets/119559917/10fab5b5-3943-482e-8f11-3f66dababddf)
```
plt.plot(x,y,'g*',linestyle='dashed',linewidth=2,markersize=12)
plt.xlabel('X axis')
plt.ylabel('Y axis')
plt.title('2d Diagram')
```
![image](https://github.com/silambarasan2004/EXNO-5-DS/assets/119559917/a8c0f7f2-87f6-41f4-9aca-fd75649041ea)
```
np.pi
```
![image](https://github.com/silambarasan2004/EXNO-5-DS/assets/119559917/eef76e04-b85a-4467-8c15-fc9c462c7fad)
```
x=np.arange(0,4*np.pi,0.1)
y=np.sin(x)
plt.title("sine wave form")
plt.plot(x,y)
plt.show()
```
![image](https://github.com/silambarasan2004/EXNO-5-DS/assets/119559917/3c306f2b-6194-4f8c-8470-2c4ffb223f50)
```
import matplotlib.pyplot as plt
import numpy as np
x=[1,2,3,4,5]
y1=[10,12,14,16,18]
y2=[5,7,9,11,13]
y3=[2,4,6,8,10]
plt.fill_between(x,y1,color='blue')
plt.fill_between(x,y2,color='green')
```
![image](https://github.com/silambarasan2004/EXNO-5-DS/assets/119559917/810db39b-28a3-4854-b69d-7ab375fce5e1)
```
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
![image](https://github.com/silambarasan2004/EXNO-5-DS/assets/119559917/2bca623b-f0ad-484d-bd82-84646c49d7b4)

```
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
![image](https://github.com/silambarasan2004/EXNO-5-DS/assets/119559917/35363c52-7763-4602-b9f6-7ed88d0e318d)
```
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
![image](https://github.com/silambarasan2004/EXNO-5-DS/assets/119559917/7a6cfbb6-bd14-4773-80bc-e8bae3aa1605)
```
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
![image](https://github.com/silambarasan2004/EXNO-5-DS/assets/119559917/29e56ffd-29e5-4fb8-83ee-8be8a5767c5c)
```
import matplotlib.pyplot as plt
import numpy as np
np.random.seed(0)
data=np.random.normal(loc=0,scale=1,size=100)
data
```
![image](https://github.com/silambarasan2004/EXNO-5-DS/assets/119559917/2f371466-aa15-4420-885b-b3b69497458d)
```
fig,ax=plt.subplots()
ax.boxplot(data)
ax.set_xlabel('Data')
ax.set_ylabel('Values')
ax.set_title('Box Plot')
```
![image](https://github.com/silambarasan2004/EXNO-5-DS/assets/119559917/a5a8b39a-15d0-4be5-8585-8f057dc87c70)

```
labels='Python','C++','Ruby','Java'
sizes=[215,130,245,210]
colors=['gold','yellowgreen','lightcoral','lightskyblue']
explode=(0,0.4,0,0.5)
plt.pie(sizes,explode=explode,labels=labels,colors=colors,autopct='%1.1f%%',shadow=True)
plt.axis('equal')
plt.show()
```
![image](https://github.com/silambarasan2004/EXNO-5-DS/assets/119559917/f103997b-875b-4a61-9ba0-47264d0b7ffb)
```
activities=['eat','sleep','work','play']
slices=[3,7,8,6]
colors=['r','y','g','b']
plt.pie(slices,labels=activities,colors=colors,startangle=90,shadow=True,explode=(0,0,0.1,0),radius=1.2,autopct='%1.1f%%')
plt.legend()
```
![image](https://github.com/silambarasan2004/EXNO-5-DS/assets/119559917/2ee460c1-f56d-44da-a605-c7069ebc9795)

# Result:
  Thus, The implementation of data visualization using matplotlib has been successfully verified.
