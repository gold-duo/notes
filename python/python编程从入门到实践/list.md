## p52-解析列表
```python
list=[]
for r in range(1,6):
    s=r**2          #两个*表示乘方
    list.append(s)
print(list)

list2=[v**2 for v in range(1,6)] ##解析列表等价于上面的
print(list2)
```

## p32-list
```python
bicycles=['trek','cannondale','redline','specialized']
bicycles.append("aaa")#添加
del bicycles[0]       #删除
bicycles.insert(2,"222")#指定位置插入
print(bicycles.pop(0)) #弹出指定位置元素
bicycles.remove("aaa") #根据值删除元素
print(sorted(bicycles,reverse=False))#排序不改变原列表，reverse排序顺序
bicycles.sort()        #排序
print(bicycles)
```