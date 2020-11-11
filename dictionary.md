# 字典

## 一个简单的字典

```python
alien_0 = {'color':'green','points':5}

print(alien_0['color'])
print(alien_0['points'])
```

### 使用字典

>字典是一系列键值对，每个键都与一个值相关联。可以使用键来访问与之相关联的值，与键相关联的可以是数字，字符串，列表甚至是字典

### 访问字典的值

```python
alien_0['color']
```

### 增加键值对

```python
alien_0['x_position'] = 0
alien_0['y_position'] = 25
```

>字典是一种动态结构，可以随时增加键值对。python不关心键-值对的增加顺序，只关心他们之间的关联

```python
alien_0 = {'color':'red','color':'green'} #没有报错，且color值为green
```

### 先创建一个空字典

```python
alien_0 = {}
alien_0['color'] = 'green'
```

### 修改字典的值

```python
alien_0['color'] = 'red'
```

```python
# 以不同速度移动的外星人的位置进行跟踪
alien_0 = {'x_positon':0,'y_postion':25,'speed':'medium'}
print('Original x_position'+str(alien_0['x_positon']))

#向右移动外星人，根据当前速度决定移动多院
if alien_0['speed'] == 'slow':
    x_increment = 1
elif alien_0['speed'] == 'meduim':
    x_increment = 2
else:
    x_increment = 3

 alien_0['x_position'] = alien_0['x_position'] + x_increment
print('New x-postion: '+ str(alien_0['x_position']))
```

### 删除键值对

```python
del alien_0['color'] #永久删除
```

### 由类似对象组成的字典

```python
favorite_languages = {
    'jen':'python',
    'sarah':'c',
    'phil':'python',
}
```



## 遍历字典

###  遍历所有的键值对

```python
user_0 = {
    'username':'eferimi',
    'first':'enrico',
    'last':'fermi',
}
for key,value in user_0.items():
    print(key)
    print(value)
```

### 遍历字典中的所有键

```python
for name in user_0.keys():
    print(name)
```

### 按顺序遍历字典中的所有键

```python
for name in sorted(user_0.keys()):
    print(name)
```

### 遍历字典中的所有值

```python
for lan in favo_lan.values():
    print(lan)
    
for lan in set(favo_lan.values()): #可以剔除重复项
    print(lan)
```

## 嵌套

> 将一系列字典存储在列表中，或将列表存储在字典中

### 字典列表

```python
alien_0 = {'color':'red','point':5}
alien_1 = {'color':'green','point':15}
alien_2 = {'color':'yellow','point':1}

aliens = [alien_0,alien_1,alien_3]

for alien in aliens:
    print(alien)
```

### 在字典中存储列表

```python
favo_lan ={
    'jen':['python','ruby'],
    'sarah':['c'],
    'edwar':['ruby','go'],
}

for key,value in favo_lan.items():
    print(key+"' favorite language is")
    if len(value) <= 1:
        print(lan)
    else:
        for lan in value:
            print(lan)

```

### 在字典中存储字典

```python
users = {
    'wy':{
        'first':'yan',
        'last':'wang',
    },
    'hm':{
        'first':'miao',
        'last':'hu',
    },
}
```

