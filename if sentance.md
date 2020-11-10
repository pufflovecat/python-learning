# if语句

## 一个简单的示例

```python
cars = ['audi','nmw','suabru']
for car in cars:
    if car == 'nmw':
        print(car.upper())
    else:
        print(car.title())
        
```

## 条件测试

### 检查是否相等

```python
car == "bmw"
```

### 检查是否相等时不考虑大小写

```
car.lower() == 'audi'
```

### 检查是否不等

```python
car != 'anchovies'
```

### 比较数字

> 等于，不等于，小于，小于等于，大于，大于等于

### 检查多个条件

> and  or

### 检查特定值是否包含在列表中

```python
num = [1,2,3,4]
1 in num 
5 not in num
```

### 布尔表达式

```python
game_active = True
can_edit = False
```

## if语句

### 简单的if语句

```python
age = 19
if age >= 18:
    print("you are old enough to vote!")
```

### if-else语句

```python
age = 17
if age >= 18:
    print("You are old enough to votel")
else:
    print("sorry,you are too young to vote.")
```

### if-elif-else结构

> 依次检查每个条件测试，直到遇到通过了的条件测试，然后跳过其他测试，继续执行后面的代码

```python
age = 12
if age < 4:
    price = 0
elif age < 18:
    price = 5
 elif age < 65:
    price = 10
 else:
    price = 5
print("You admission const is $"+ str(price)+'.')
```

### 省略else代码块

>else是一条包罗万象的语句，代码这样会引入无效甚至恶意的数据，如果知道最终要测试的条件，应考虑使用一个elif语句

### 测试多个条件

```python
nums = [1,2,3]
if 1 in nums:
    print(1)
if 2 in nums:
    print(2)
if 3 in nums:
    print(3)
```

> 如果这里用if-elif的格式，代码是不正确的，因为他遇到一个测试通过后就会跳过其他测试。所以如果只想执行一个代码块，就用if-elif-else结构；如果想要运行多个代码块，就用一系列独立的If语句

## 使用if语句处理列表

### 检查特殊元素

```python
nums = [1,2,3]
for num in nums:
    if num == 1:
        print("ok")
    else:
        print("fine")
```

### 确定列表不是空

```python
nums = []
if nums :
    for num in nums:
        print(num)
else:
    print("Please enter number")
```

### 使用多个列表

```python
nums = [1,2,3,4,5]
nums_req = [1,2,3]
if nums_req :
    for num_req in nums_req :
        if num_req in nums:
            print("ok")
         else:
            print("we don't have")
 else:
    print("Please enter number")
```

