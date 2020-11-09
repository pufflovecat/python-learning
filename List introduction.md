# 列表简介

## 列表是什么

> 由一些列按特定顺序排列的元素组成，元素之间没有任何联系。用[ ]表示，且用逗号分隔其中的元素

```python
bicycles = ['trek','reline','specialized']
```

### 访问列表元素

> 列表是有序集合，因此要访问列表的任何元素，只需将该元素的位置或者索引告诉Python

```python
print(bicycles[0].title())
```

### 索引从0开始而不是从1

```python
print(bicycles[-1]) #打印最后一个
```

### 使用列表中的各个值

> 可以像使用变量一样使用列表中的各个值

## 修改，增加和删除元素

### 修改列表元素

> 修改列表元素的语法与访问列表元素语法类似，指定列表名和要修改的元素索引，再赋值新值

```python
name = ['zs','ls','wy']
name[0] = 'hm'
```

### 在列表中增加元素

#### 在末尾增加

```python
names = []
names.append("wy")
names.append('zs')
```

#### 在列表中增加

```python
names.insert(0,'ls')
```

### 列表删除元素

#### 使用del语句删除元素

如果知道元素的位置，就能使用del语句

```python
del names[0]
```

#### 使用方法pop()删除元素

删除末尾的元素且可以继续使用

```python
name = names.pop()
```

#### 弹出列表中任何位置的元素

```python
name = names.pop(0)
```



> 如果要从列表删除一个元素，如果不再使用就用del；以后继续使用用pop()

#### 根据值删除元素

如果不知道列表中删除值所在处就用remove()

```python
names.remove('wy')
```

> remove（）方法只能删除第一个指定值，如果删除的值在列表中出现多次，就需要循环来判断

### 组织列表

调正列表排列顺序，同时又保留原来的顺序

#### 使用sort()方法对列表永久排序

```python
num = [2,1,4,3]
num.sort() #升序
print(num)
num.sort(reverse = True) #降序

```

#### 使用函数sorted()对列表进行临时排序

```python
print(sorted(num))
print(num)
```

### 倒着打印列表

反转列表元素的排列顺序

```python
num.reverse()
```

#### 确定列表的长度

使用函数len()

```python
len(num)
```

#### 使用列表时避免出现索引错误

>发生索引错误却找不到解决方法时，尝试将列表或者其长度打印出来。