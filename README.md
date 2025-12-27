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
 import pandas as pd
import numpy as np
import seaborn as sns
import matplotlib.pyplot as plt
```

LINE PLOT

```
marks=[13,45,63,78]
student=['ABC','QOR','EFB','TOB']
plt.plot(marks,student)
plt.xlabel('Marks')
plt.ylabel('Student name')
plt.show()
student=['A','B','C','D']
attendence=[90,85,73,88]
plt.plot(attendence,student)
plt.xlabel('Attendence')
plt.ylabel('Student name')
plt.show()

```
<img width="821" height="551" alt="image" src="https://github.com/user-attachments/assets/6e559e21-f811-4a3d-809e-797ba4602cd7" />     <img width="800" height="556" alt="image" src="https://github.com/user-attachments/assets/f242dcd9-3e26-489f-899d-e3455338044d" />


SCATTER PLOT 
```
x=[10,20,30,40,50]
y=[100,200,300,400,500]
plt.scatter(x,y,label='stars',color='green',marker='*',s=30)
plt.show()
x=np.arange(0,15)
y=np.arange(0,15)
x
y
plt.scatter(x,y,c='r')
plt.xlabel('X axis')
plt.ylabel('y axis')
plt.title('Scatter plot')
plt.show()
```

<img width="743" height="522" alt="image" src="https://github.com/user-attachments/assets/42e16bc9-be51-4dc0-8643-972bf7ae9612" />    <img width="758" height="560" alt="image" src="https://github.com/user-attachments/assets/c16ff6e8-f156-41a7-97d9-83b1206dc2e0" />


PIE CHART 
```
act=['eat','sleep','work','play']
slices=[3,7,8,6]
color=['r','y','g','b']
plt.pie(slices,labels=act,colors=color,startangle=90,shadow=True,explode=(0.1,0.1,0.1,0.1),radius=1.2,autopct='%1.1f%%')
plt.legend()
plt.show()
feedback=['Good','excellent','Perfect','Ok']
slices=[4,10,3,8]
color=['y','r','b','g']
plt.pie(slices,labels=feedback,colors=color,startangle=90,shadow=True,explode=(0.1,0.1,0.1,0.1),radius=1.2,autopct='%1.1f%%')
plt.legend()
plt.show()
```

<img width="701" height="517" alt="image" src="https://github.com/user-attachments/assets/cb3fa9ec-6fe4-4cf7-829b-bd2fd606b883" />   <img width="704" height="524" alt="image" src="https://github.com/user-attachments/assets/896ae453-9717-47cb-82cf-de70fce4bbb1" />


AREA CHART 
```
x = [1, 2, 3, 4, 5]
y1 = [10, 12, 14, 16, 18]
y2 = [5, 7, 9, 11, 13]
y3 = [2, 4, 6, 8, 10]
plt.fill_between(x, y1, color='blue')
plt.fill_between(x, y2, color='green')
plt.plot(x, y1, color='red')
plt.plot(x, y2, color='black')
plt.legend(['y1','y2'])
plt.show()
```

<img width="749" height="528" alt="image" src="https://github.com/user-attachments/assets/c7377e61-0c65-4035-95e1-a4fe75591e60" />


BAR CHART 
```
height = [10, 24, 36, 40, 5]
names = ['one', 'two', 'three', 'four', 'five']
c1=['red', 'green']
c2=['b', 'g']
plt.bar (names, height, width=0.8, color=c1)
plt.xlabel('x - axis')
plt.ylabel('y - axis')
plt.title('My bar chart!')
plt.show()
```

<img width="786" height="572" alt="image" src="https://github.com/user-attachments/assets/2020719d-65e3-465a-bfc7-ac3f5d5b3c23" />


HISTOGRAM 
```
x = [2,1,6,4,2,4,8,9,4,2,4,10,6,4,5,7,7,3,2,7,5,3,5,9,2,1]
plt.hist(x, bins = 10, color='blue', alpha=0.5)
plt.show()
```

<img width="730" height="524" alt="image" src="https://github.com/user-attachments/assets/53631467-ec3c-4248-b59d-d9b85bdedbdc" />

BOX PLOT 
```
np.random.seed(0)
data=np.random.normal(loc=0, scale=1, size=100)
data
```

<img width="737" height="449" alt="image" src="https://github.com/user-attachments/assets/0f11576f-0d63-46e1-ac75-0175d59f0a83" />

```
fig, ax= plt.subplots()
ax.boxplot(data)
ax.set_xlabel('Data')
ax.set_ylabel('Values')
ax.set_title('Box Plot')
```

<img width="772" height="593" alt="image" src="https://github.com/user-attachments/assets/57401d8f-ac2b-4925-994d-86f9ca2a7219" />


# Result:
 Include your result here
