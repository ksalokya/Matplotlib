<div align="center">
  <img src="https://github.com/matplotlib/matplotlib/blob/main/doc/_static/matplotlib-icon.svg" width="300px"/>
</div>
<h1 align="center">Matplotlib Cheatsheet</h1>

# Importing library


```python
%matplotlib inline
import matplotlib as plt
```

# Importing particular package


```python
from matplotlib import pyplot as plt
plt.plot([1,2,3], [4,5,7])
plt.show()
```


    
![png](https://github.com/ksalokya/matplotlib/blob/main/assets/output_3_0.png)
    


# Heading & Axis


```python
from matplotlib import pyplot as plt
plt.plot([1,2,3], [4,5,7])
plt.title("Sample Data")
plt.xlabel("X")
plt.ylabel("Y")
plt.show()
```


    
![png](https://github.com/ksalokya/matplotlib/blob/main/assets/output_5_0.png)
    


# Changing Style


```python
from matplotlib import pyplot as plt
from matplotlib import style

style.use('ggplot')
x1 = [1,5,4]
y1 = [23,45,89]
x2 = [3,7,3]
y2 = [5,8,9]

plt.plot(x1,y1)
plt.plot(x2,y2)

plt.show()
```


    
![png](https://github.com/ksalokya/matplotlib/blob/main/assets/output_7_0.png)
    


# Label


```python
from matplotlib import pyplot as plt
from matplotlib import style

style.use('ggplot')
x1 = [1,5,4]
y1 = [23,45,89]
x2 = [3,7,3]
y2 = [5,8,9]

plt.plot(x1,y1,label='first')
plt.plot(x2,y2,label='second')
plt.legend()
plt.show()
```


    
![png](https://github.com/ksalokya/matplotlib/blob/main/assets/output_9_0.png)
    


# Line Width


```python
from matplotlib import pyplot as plt
from matplotlib import style

style.use('ggplot')
x1 = [1,5,4]
y1 = [23,45,89]
x2 = [3,7,3]
y2 = [5,8,9]

plt.plot(x1,y1,label='first',linewidth=8)
plt.plot(x2,y2,label='second',linewidth=4)
plt.legend()
plt.show()
```


    
![png](https://github.com/ksalokya/matplotlib/blob/main/assets/output_11_0.png)
    


# Scatter Plot


```python
from matplotlib import pyplot as plt
from matplotlib import style

style.use('ggplot')
x1 = [1,5,4]
y1 = [23,45,89]
x2 = [3,7,3]
y2 = [5,8,9]

plt.scatter(x1,y1,label='first')
plt.scatter(x2,y2,label='second')
plt.legend()
plt.show()
```


    
![png](https://github.com/ksalokya/matplotlib/blob/main/assets/output_13_0.png)
    


# Histogram


```python
from matplotlib import pyplot as plt

x1 = [1,1,1,1,4,4,4,4,5,4,3,5,5,5,5,2,2,2,2]

plt.hist(x1)
plt.show()
```


    
![png](https://github.com/ksalokya/matplotlib/blob/main/assets/output_15_0.png)
    


# Pie chart


```python
import matplotlib.pyplot as plt
import numpy as np

labels = ['Mon', 'Tue', 'Wed', 'Thu', 'Fri', 'Sat', 'Sun']

data = np.random.rand(7) * 100

plt.pie(data, labels=labels, autopct='%1.1f%%')
plt.axis('equal')
plt.legend()

plt.show()
```


    
![png](https://github.com/ksalokya/matplotlib/blob/main/assets/output_17_0.png)
    



# Bar Graphs


```python
plt.bar([0,1,2],[10,20,15])
plt.show()
```


    
![png](output_19_0.png)
    



```python
import numpy as np
x_cord = np.array(np.arange(3))
plt.bar(x_cord ,[10,20,15],width=0.5)
plt.bar(x_cord+0.5 ,[20,10,12],width=0.5)
plt.show()
```


    
![png](output_20_0.png)
    


# Save Plot


```python
from matplotlib import pyplot as plt

x1 = [1,1,1,1,4,4,4,4,5,4,3,5,5,5,5,2,2,2,2]
plt.boxplot(x1)
plt.savefig('foo.png')
```


    
![png](output_22_0.png)
    
    

## Tutorial
[Matplotlib Tutorial](https://youtu.be/VFsRLjSc8GA)
