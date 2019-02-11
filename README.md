# Matplotlib-basic-guidance
Matplotlib 的基本用法

**1. 创建 fig 和 axes:**
```
fig, ax = plt.subplots(nrows=2, ncols=2, figsize=(16,10)) # 两行两列共4个子图
```
notice: 当图只有一行时,例如一行两列或者三列, 那么每个图不能用两个数字表示,而应该用一个数字,例如 ```ax[0], ax[1]```

**2.1 线形图**
```
ax[0,0]. plot(x, y)
```
**2.2 散点图**
```
ax[0,1].scatter(x,y)
```
**2.3 条形图**
```
ax[1,0].bar(x,y)
ax[1,0].barh(x,y) 
```
**2.4 饼状图**
```
ax[1,1].pie()
```

**3. 图设置**
```
ax.set(title='', xlabel='', ylebel='') #整体设置
ax.title()  # 设置图名
ax.xlim() #设置轴参数
ax.ylim()
ax.xlabel() #设置轴名
ax.ylabel()
ax.legend() #添加图注

ax.text() #添加 text
