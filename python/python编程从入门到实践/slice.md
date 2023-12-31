## p54-slice
```python
players=['charles', 'martina','michael','florence','eli']
print(players[1:3])#list[start:end],不包含end索引对应元素
print(players[:3])#不指定start索引默认从0开始
print(players[1:])#不指定end索引默认到结束
print(players[:])#start和end都不指定复制列表
print(players[-3:])#start为负数返回最后start个元素
```