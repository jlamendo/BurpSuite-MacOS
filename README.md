BurpSuite-MacOS
===============
![](http://mweb.03sec.com/2018-01-26-15169456970441.jpg)

# 编译BurpSuite破解版为Mac Applocation

## 一、系统环境
### java
 安装步骤：
 
 。。。。不知道如何安装java，那就放弃吧！新版本burp要求最低jdk8以上
### ant
#### 安装步骤

安装brew

```
https://brew.sh/
```
brew 执行安装命令

```
brew install ant

```
 


## 二、详细步骤
首先从github上下载代码：

```
git clone https://github.com/iusky/BurpSuite-MacOS
```

然后进入该目录,直接执行

```
ant bundle
```
![](http://mweb.03sec.com/2018-01-26-15169455640146.jpg)

然后会在当前目录下生成一个名字为

```
Burp Suite Professional.app
```
的应用
![](http://mweb.03sec.com/2018-01-26-15169454570028.jpg)


## 三、更改了哪些参数？

1、更改了build.xml文件里面的mainclassname,将其改为了burploader的启动函数
2、将burp破解版的程序拷贝到了当前目录
3、更改了icon图标

## 四、新版本激活步骤
1. 打包好app用户，请直接双击打开应用，此时是未激活的状态
![](http://mweb.03sec.com/2018-01-26-15169447609665.jpg)

2. 双击打开burp-loader-keygen.jar，根据自己的需求修改License text的内容，然后将License文本框里面生成的一大串key复制出来，保存为一个文件
![](http://mweb.03sec.com/2018-01-26-15169447851635.jpg)
![](http://mweb.03sec.com/2018-01-26-15169447969534.jpg)

3. 在第一步中打开app后，选择key文件为激活文件
![](http://mweb.03sec.com/2018-01-26-15169448151197.jpg)
![](http://mweb.03sec.com/2018-01-26-15169448507785.jpg)
![](http://mweb.03sec.com/2018-01-26-15169448553134.jpg)

4. 然后点击下一步
![](http://mweb.03sec.com/2018-01-26-15169451271421.jpg)
然后选择Manual activation
5. 复制request到keygen里面的activation request文本框内，![](http://mweb.03sec.com/2018-01-26-15169451887661.jpg)
![](http://mweb.03sec.com/2018-01-26-15169452080793.jpg)
6. 复制activation response的内容到第四步的response里面
![](http://mweb.03sec.com/2018-01-26-15169452836490.jpg)
7. 点击下一步，激活成功
![](http://mweb.03sec.com/2018-01-26-15169453416766.jpg)
![](http://mweb.03sec.com/2018-01-26-15169453941798.jpg)


