# 列表的操作

## 遍历整个列表

### 深入研究循环

```python
magicians = ['alice','david','carolina']
for magician in magicians: # 从magicians中获取值，并存在magician中
    print(magician)
```

> 存储列表中每个值的临时变量，可以指定任何名称，但是最好选择对列表有描述性的

### 在for循环中执行更多操作

```python
for num in nums:
    print(num + " is my favorite number.")
    print("I am "+ num+" years old.\n")
```

> 循环中可以包含任何行代码

### 在for循环结束后执行的一些操作

> 在for循环后，没有缩进的代码只执行一次

## 避免缩进错误

* 忘记缩进
* 忘记缩进额外的代码行
* 不必要的缩进
* 循环后不必要的缩进
* 遗漏了冒号

## 创建数值列表

###  使用range()函数

```python
for value in range(1,5):
    print(value)
```

> range()从指定第一个数字开始，并在指定第二个值前停止

### 使用range()创建数字列表

```python
nums = list(range(1,6))
nums = list(range(2,11,2))#还可以指定步长
```



```python
nums = []
for value in range(1,11):
    nums.append(value**2)
print(nums)
   
```



### 对数字列表执行简单的统计计算

```python
min(nums)
max(nums)
sum(nums)
```

### 列表解析

```python
squares = [value**2 for value in range(1,11)]
print(squares)
```

## 使用列表的一部分

### 切片

```python
print(nums[1:4])
print(nums[1:])
print(nums[:4])
print(nums[-3:])#打印后三个
```

### 遍历切片

```python
for i in num[1:5]:
    print(i)
```

### 复制列表

```python
num = nums #这俩同步
num = nums[:] #这俩不同步
```

## 元组

> 值不可变的列表

### 定义元组

```python
nums = (1,3)
```

### 遍历元组中的值

```python
for num in nums:
    print(num)
```

### 修改元组变量

```python
nums = (3,4)
```

> 不能修改元组中的元素，但是可以改变整体赋值

## 设置代码格式

* 每级缩进使用四个空格
* 每行不超过80字符
* 不要在文件中使用过多空行