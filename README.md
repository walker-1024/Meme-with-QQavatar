# Meme-with-QQavatar

## 简介

给定一个QQ号和指令，将获取其头像，制作成为一个有趣的表情包。非常适合作为QQbot的一个功能。



## 功能

### 丢

<img src="result/1641818404.12908.jpg" alt="1641818404.12908" width = "500" />

<img src="result/1641818404.1976929.gif" alt="1641818404.1976929" width = "500" />

<img src="result/1642313462.4174132.gif" alt="1642313462.4174132" width = "500" />

### 仰望大佬

<img src="result/1641818404.445751.jpg" alt="1641818404.445751" width = "500" />

### 打拳

<img src="result/1641818404.78143.gif" alt="1641818404.78143" width = "500" />

### 打

<img src="result/1641818405.057256.gif" alt="1641818405.057256" width = "500" />

<img src="result/1641818405.070693.gif" alt="1641818405.070693" width = "500" />

### 摸头

<img src="result/1641818405.300173.gif" alt="1641818405.300173" width = "500" />

### 摸鱼

<img src="result/1641818405.589279.png" alt="1641818405.589279" width = "500" />

<img src="result/1641818405.6541681.gif" alt="1641818405.6541681" width = "500" />

### 摸

<img src="result/1641818405.9694002.gif" alt="1641818405.9694002" width = "500" />

### 敲

<img src="result/1641818406.2234979.gif" alt="1641818406.2234979" width = "500" />

<img src="result/1641818406.229162.gif" alt="1641818406.229162" width = "500" />

### 赞

<img src="result/1641818406.523747.gif" alt="1641818406.523747" width = "500" />

### 旋转

<img src="result/1641818406.925292.gif" alt="1641818406.925292" width = "500" />

### 吃

<img src="result/1641818407.28931.png" alt="1641818407.28931" width = "500" />

<img src="result/1642485824.8275259.jpg" alt="1642485824.8275259" width = "500" />

### 吞

<img src="result/1641818407.776714.gif" alt="1641818407.776714" width = "500" />

### 咬

<img src="result/1641818408.141077.gif" alt="1641818408.141077" width = "500" />

### 快逃

<img src="result/1641818408.343437.gif" alt="1641818408.343437" width = "500" />

### 色色

<img src="result/1641818408.6079512.gif" alt="1641818408.6079512" width = "500" />

### 舔

<img src="result/1641818408.8851242.gif" alt="1641818408.8851242" width = "500" />

### 拍

<img src="result/1641818409.1798348.gif" alt="1641818409.1798348" width = "500" />

### 爬

<img src="result/1641818409.381533.jpg" alt="1641818409.381533" width = "500" />

### 推

<img src="result/1641818409.831573.gif" alt="1641818409.831573" width = "500" />

### 踢

<img src="result/1641818410.256871.gif" alt="1641818410.256871" width = "500" />

### 捂脸

<img src="result/1642313467.541203.png" alt="1642313467.541203" width = "500" />

### 踩

<img src="result/1642394725.157651.gif" alt="1642394725.157651" width = "500" />

### 脆弱

<img src="result/1651169640.8554251.png" alt="1651169640.8554251" width = "500" />

### There will be more...



## 使用

### 依赖

- requests
- pillow

### 代码

``` python
testQQNum = 10000

# 格式应为：丢[@QQ号] 或者 丢QQ号
# 其中的 "丢" 表示要画 "丢" 这张图，可以换成其他指令
# 之所以支持 "[@QQ号]" 的格式是因为在大多数 qqbot 框架中，消息中的艾特是这种格式

testCommand = [
    "丢{}".format(testQQNum),
    "仰望大佬{}".format(testQQNum),
    "打拳{}".format(testQQNum),
    "打{}".format(testQQNum),
    "摸头{}".format(testQQNum),
    "摸鱼{}".format(testQQNum),
    "摸{}".format(testQQNum),
    "敲{}".format(testQQNum),
    "赞{}".format(testQQNum),
    "旋转{}".format(testQQNum),
    "吃{}".format(testQQNum),
    "吞{}".format(testQQNum),
    "咬[@{}]".format(testQQNum),
    "快逃[@{}]".format(testQQNum),
    "色色[@{}]".format(testQQNum),
    "舔[@{}]".format(testQQNum),
    "拍[@{}]".format(testQQNum),
    "爬[@{}]".format(testQQNum),
    "推[@{}]".format(testQQNum),
    "踢[@{}]".format(testQQNum),
    "捂脸[@{}]".format(testQQNum),
    "踩[@{}]".format(testQQNum),
    "脆弱{}".format(testQQNum),
]

tool = DrawTool()
for command in testCommand:
    result = tool.wantDraw(command)
    if result != None:
        # 如果成功的话，将拿到一个数组，里面是每个结果图片的本地绝对路径，有的命令会生成多张图
        print(result)
```



## 感谢

<img src="pawaluodi.png" alt="pawaluodi" width = "50" />  怕瓦落地



