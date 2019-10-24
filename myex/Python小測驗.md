# 程式設計題
```
for 迴圈(loop)的技巧
1.使用for 迴圈(loop)計算1+2+3+.....100
2.使用for 迴圈(loop)計算1+3+5+7.....+99
3.使用for 迴圈(loop)計算1*3*5*7.....*99

while 迴圈(loop)的技巧
4.使用while 迴圈(loop)計算1+2+3+.....100
5.使用while 迴圈(loop)計算1+3+5+7.....+99
6.使用while 迴圈(loop計算1*3*5*7.....*99
```


# 程式設計題解答(有各種寫法,找寫最快的分數最高)

### 使用for 迴圈(loop)計算1+2+3+.....100
```
sum=0

for x in range(1,101):
  sum +=x
  
print(sum)
```
### 使用for 迴圈(loop)計算1+3+5+7.....+99
```
sum=0

for x in range(1,101,2):
  sum +=x
  
print(sum)
```
### 使用for 迴圈(loop)計算
```
1*3*5*7.....*99
```
```
total=1

for x in range(1,101,2):
  total *=x
  
print(total)
```

### 使用while 迴圈(loop)計算1+2+3+.....100
```
sum = 0
x=1

while x < 101:
  sum +=x
  x = x+1
  # x += 1
  
print(sum)
```
### 使用while 迴圈(loop)計算1+3+5+7.....+99
```
sum = 0
x=1

while x < 101:
  sum +=x
  x = x+2
  # x += 1
  
print(sum)
```

### 使用while 迴圈(loop)計算
```
1*3*5*7.....*99
```
```
total = 1
x=1

while x < 101:
  total *=x
  x = x+2     # x += 2
  
print(total)
```
