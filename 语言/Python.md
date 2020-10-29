1. 推倒式
https://www.cnblogs.com/zknublx/p/9534346.html

2. 括号
语言最常见的括号有三种，分别是：小括号( )、中括号[ ]和大括号也叫做花括号{ }，分别用来代表不同的python基本内置数据类型。

    - python中的小括号( )：代表tuple元组数据类型，元组是一种不可变序列。
 ```
>>> tup = (1,2,3)    
>>> tup    
(1, 2, 3)    
````

    - python中的中括号[ ]，代表list列表数据类型：
 ```
>>> list('python')    
['p', 'y', 't', 'h', 'o', 'n']
````
    - python大括号{ }花括号：代表dict字典数据类型，字典是由键对值组组成。冒号':'分开键和值，逗号','隔开组。用大括号创建的方法如下：
 ```
>>> dic={'jon':'boy','lili':'girl'}    
>>> dic    
{'lili': 'girl', 'jon': 'boy'}    
>>>
````

3. set frozenset

set(可变集合)与frozenset(不可变集合)的区别：
set无序排序且不重复，是可变的，有add（），remove（）等方法。既然是可变的，所以它不存在哈希值。基本功能包括关系测试和消除重复元素. 集合对象还支持union(联合), intersection(交集), difference(差集)和sysmmetric difference(对称差集)等数学运算.
sets 支持 x in set, len(set),和 for x in set。作为一个无序的集合，sets不记录元素位置或者插入点。因此，sets不支持 indexing, 或其它类序列的操作。
frozenset是冻结的集合，它是不可变的，存在哈希值，好处是它可以作为字典的key，也可以作为其它集合的元素。缺点是一旦创建便不能更改，没有add，remove方法。

4. sorted

sorted() 函数对所有可迭代的对象进行排序操作。
sort 与 sorted 区别：
    - sort 是应用在 list 上的方法，sorted 可以对所有可迭代的对象进行排序操作。
list 的 sort 方法返回的是对已经存在的列表进行操作，无返回值，而内建函数 sorted 方法返回的是一个新的 list，而不是在原来的基础上进行的操作。
     - sorted(iterable, cmp=None, key=None, reverse=False)
参数说明：
iterable -- 可迭代对象。
cmp -- 比较的函数，这个具有两个参数，参数的值都是从可迭代对象中取出，此函数必须遵守的规则为，大于则返回1，小于则返回-1，等于则返回0。
key -- 主要是用来进行比较的元素，只有一个参数，具体的函数的参数就是取自于可迭代对象中，指定可迭代对象中的一个元素来进行排序。
reverse -- 排序规则，reverse = True 降序 ， reverse = False 升序（默认）。
```
>>>a = [5,7,6,3,4,1,2]
>>> b = sorted(a) # 保留原列表
>>> a 
[5, 7, 6, 3, 4, 1, 2]
>>> b
[1, 2, 3, 4, 5, 6, 7] 
>>> L=[('b',2),('a',1),('c',3),('d',4)]
>>> sorted(L, cmp=lambda x,y:cmp(x[1],y[1])) # 利用cmp函数
[('a', 1), ('b', 2), ('c', 3), ('d', 4)]
>>> sorted(L, key=lambda x:x[1]) # 利用key[('a', 1), ('b', 2), ('c', 3), ('d', 4)] 
>>> students = [('john', 'A', 15), ('jane', 'B', 12), ('dave', 'B', 10)]
>>> sorted(students, key=lambda s: s[2]) # 按年龄排序
[('dave', 'B', 10), ('jane', 'B', 12), ('john', 'A', 15)] 
>>> sorted(students, key=lambda s: s[2], reverse=True) # 按降序
[('john', 'A', 15), ('jane', 'B', 12), ('dave', 'B', 10)]
```
5. 
