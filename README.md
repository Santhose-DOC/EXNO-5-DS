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

 NAME : SANTHOSE AROCKIARAJ J
 
 REG NO : 212224230248

 ### DATA VISUALIZATION
 ```
import matplotlib.pyplot as plt
x1=[1,2,3]
y1=[2,4,1]
plt.plot(x1,y1,label='Line1',linewidth=6)
x2=[1,2,3]
y2=[4,1,3]
plt.plot(x2,y2,label="Line2",linewidth=6)
plt.xlabel("x-AXIS")
plt.ylabel("Y-AXIS")
plt.title("Two lines on same graph")
plt.legend()
```
![image](https://github.com/user-attachments/assets/51cad45f-681f-42ed-9ded-08c554ef933f)
```
import matplotlib.pyplot as plt
x=[1,2,3,4,5,6]
y=[2,4,1,5,2,6]

plt.plot(x,y,color='blue',linestyle='dashed',linewidth=4,marker='o',markerfacecolor='red',markersize=14)
plt.ylim(1,8)
plt.xlim(1,8)
plt.xlabel("X-AXIS")
plt.ylabel("Y-AXIS")
plt.title("Some coll customizations")
```
![image](https://github.com/user-attachments/assets/1c7cffc0-2bdf-41a2-bf12-708c09e6c4e4)
```
years=range(2000,2012)
apples=[0.895,0.91,0.919,0.926,0.929,0.931,0.934,0.936,0.937,0.9375,0.9372,0.939]
oranges=[0.962,0.947,0.930,0.923,0.918,0.908,0.907,0.904,0.901,0.898,0.9,0.896]
plt.plot(years,apples,color='red',linewidth=5)
plt.plot(years,oranges,color='orange',linewidth=5)
plt.xlabel('YEar')
plt.ylabel("Yielss (tons per hectare)")
plt.title("Crop yield in Kanto")
plt.legend(['Apples','Oranges'])
```
![image](https://github.com/user-attachments/assets/339e7da6-ea88-4da7-b028-85d286de2e48)
```
import matplotlib.pyplot as plt
x_values=[0,1,2,3,4,5]
y_values=[0,1,4,9,16,25]
plt.scatter(x_values,y_values,s=100,c='red')
plt.xlabel("X-AXIS")
plt.ylabel("Y-AXIS")
plt.title("Scatter Plot")
```
![image](https://github.com/user-attachments/assets/cc94bdf4-84a1-45a0-8117-66568f38738c)
```
import matplotlib.pyplot as plt
x=[1,2,3,4,5,6,7,8,9,10]
y=[2,4,5,7,6,8,9,11,12,12]
plt.scatter(x,y,label='stars',marker="*",s=300,c="blue")
plt.xlabel("X-AXIS")
plt.ylabel("Y-AXIS")
plt.title("Scatter Plot Star")
plt.legend()
plt.savefig("StartScatter.png")
```
![image](https://github.com/user-attachments/assets/daabe776-b85c-4e04-b967-7667713ebd53)
```
import matplotlib.pyplot as plt
x=[1,2,3,4,5,6,7,8,9]
y=[1,4,9,16,25,36,47,64,81]
plt.xlabel("X-AXIS")
plt.ylabel("Y-AXIS")
plt.title("Scatter Plot")
plt.subplot(2,2,1)
plt.plot(x,y,'ro--')
plt.subplot(2,2,2)
plt.plot(y,x,'g*--')
plt.subplot(2,2,3)
plt.plot(x,x,'bo')
plt.subplot(2,2,4)
plt.plot(y,y,'go')
```
![image](https://github.com/user-attachments/assets/1c3ae545-d0cf-4822-9b49-41711a69dc3b)
```
import numpy as np
np.pi
```
![image](https://github.com/user-attachments/assets/dd8e8ebd-8e44-4128-b585-f78083870094)
```
X=np.arange(0,4*np.pi,0.1)
Y=np.sin(X)
plt.title("Sine Wave Form")
plt.plot(X,Y,linewidth=5,c="green",linestyle='dotted')
```
![image](https://github.com/user-attachments/assets/77c5badf-2205-4c62-9ebd-3d5b50ae53cf)
```
import matplotlib.pyplot as plt
import numpy as np
x=[1,2,3,4,5]
y1=[10,12,14,16,18]
y2=[5,7,9,11,13]
y3=[2,4,6,8,10]
plt.fill_between(x,y1,color='red')
plt.fill_between(x,y2,color='blue')
plt.plot(x,y1,color='black')
plt.plot(x,y2,color='white')
plt.legend(['y1','y2'])
plt.show()
```
![image](https://github.com/user-attachments/assets/abd0089a-d4bb-46bc-aaef-e5c0fdf482ab)
```
import matplotlib.pyplot as plt
height=[10,24,36,40,5]
names=['One','Two','Three','Four','Five']
c1=['g','b']
plt.bar(names,height,width=0.8,color=c1)
plt.xlabel('X-AXIS')
plt.ylabel('Y-AXIS')
plt.title('Bar Graph')
```
![image](https://github.com/user-attachments/assets/f3233193-9726-4dd7-a360-8380f3f84170)
```
x=[2,8,10]
y=[11,16,9]
x2=[3,9,11]
y2=[6,15,7]
plt.bar(x,y,color='r')
plt.bar(x2,y2,color='y')
plt.xlabel('X-AXIS')
plt.ylabel('Y-AXIS')
plt.title('Bar Graph')
```
![image](https://github.com/user-attachments/assets/8d7fd87b-4d58-40a0-b506-00c84c327344)
```
import matplotlib.pyplot as plt
x=[2,1,6,4,2,4,8,9,4,2,4,10,6,4,5,7,7,3,2,7,5,3,5,9,2,1]
plt.hist(x,bins=10,color='grey',alpha=0.5)
plt.show()
```
![image](https://github.com/user-attachments/assets/e5eb2ee5-ba16-47c4-8c91-094490a7cf73)
```
import matplotlib.pyplot as plt
import numpy as np
np.random.seed(0)
data=np.random.normal(loc=0,scale=1,size=100)
data
```
![image](https://github.com/user-attachments/assets/42dce96d-b1cf-43ee-bd6d-4f3644fd2714)
```
fig,ax=plt.subplots()
ax.boxplot(data)
ax.set_xlabel('Data')
ax.set_ylabel('Value')
ax.set_title('Box Plot')
plt.show()
```
![image](https://github.com/user-attachments/assets/53eb4708-9802-45a9-8725-c7f27f8fd41e)
```
import matplotlib.pyplot as plt
activities=['Eat','Sleep','Work','Play']
slices=[3,7,8,6]
colors=['yellow','blue','orange','red']
plt.pie(slices,labels=activities,colors=colors,startangle=90,shadow=True,explode=(0,0.1,0,0),autopct='%1.1f%%')
plt.title('Pie Chart')
plt.show()
```
![image](https://github.com/user-attachments/assets/ea75503d-685c-47bf-9400-07ba245b318f)
```
labels=['Python','C++','Ruby','Java']
sizes=[215,130,245,210]
colors=['yellow','blue','orange','red']
explode=(0.1,0,0.1,0)
plt.pie(sizes,labels=labels,colors=colors,explode=explode,shadow=True,autopct='%1.1f%%',startangle=90)
plt.title('Pie Chart')
plt.show()
```
![image](https://github.com/user-attachments/assets/84df0a76-2b5e-40de-8015-3b1d581584c8)

# Result:
Thus, performed Data Visualization using matplot python library for the given datas.

