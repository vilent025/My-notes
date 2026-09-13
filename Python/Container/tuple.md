"""
元组同列表一样都是可以封装多个、不同类型的元素在内
不同在：元组一旦定义完成，就不可修改

元组的定义：
1.字变量
(元素1，元素2,...)
2.定义变量
变量名称 = (元素1，元素2，...)
3.定义空列表
变量名称 = ()
变量名称 = tuple()

如果元组只有一个元素，要在元素后加一个逗号
t1 = ("hello",)

元组的嵌套：
    t2 = ((1,2,3),(4,5,6),(7,8,9))

支持下标索引

"""
"""
元组相关操作：

查找元素ele的下标：
    index = tuple.index(ele)

统计某元素ele的数量:
    tuple.count(ele)
    
统计元组元素数量
    len(tuple)
    
遍历一个元组
#while
index = 0
while index < len(tuple):
    print(tuple[index])
    index += 1

#for
for ele in tuple:
    print(ele)

"""
t = (1,2,3,4,5,6,7,8,9)
for i in t:
    print(i,end=" ")

