# MD学习
# [.MD语法入门](https://www.jianshu.com/p/399e5a3c7cc5 "链接") #
## 一、基本符号：* - +. >
基本上所有的markdown标记都是基于这四个符号或组合。
需要注意的是，如果以基本符号开头的标记，注意基本符号后有一个用于分割标记符和内容的空格。
例如：井号+空格+一级标题+空格+井号

## 二、标题 ##
### 1.前面带#号，后面带文字，分别表示h1-h6,只到h6，而且h1下面会有一条横线
```
# 一级标题
## 二级标题
### 三级标题
#### 四级标题
##### 五级标题
###### 六级标题
```
### 2.相当于标签闭合
```
# 一级标题 # 
## 二级标题 ## 
### 三级标题 ### 
#### 四级标题 #### 
##### 五级标题 ##### 
###### 六级标题 #####
```
六级标题效果图
![六级标题效果图](MD%E5%AD%A6%E4%B9%A0.assets/354200717226963.png)

## 三、字体格式
### 1.强调字体
一个星号或者是一个下划线包起来，会转换为<em>倾斜，如果是2个，会转换为<strong>加粗
```
*md*    
**md**
_md_   
 __md__
```
强调字体效果图
![强调字体效果图](MD%E5%AD%A6%E4%B9%A0.assets/360763909236354.png)

### 2.转义
和其他常用转义方式一样,\加需要转义的字符
```
\\
\*
\+
\-
\`
\_
```
转义效果图
![转义效果图](MD%E5%AD%A6%E4%B9%A0.assets/28414009232108.png)

### 3.删除线
用~~把需要显示删除线的字符包裹起来
```
~~删除~~
```
删除线效果图
![删除线效果图](MD%E5%AD%A6%E4%B9%A0.assets/188144009249988.png)

## 四、分割线
分割线可以由* - _（星号，减号，底线）这3个符号的至少3个符号表示，注意至少要3个，且不需要连续，有空格也可以
```
---
- - -
------
***
* * *
******
___
_ _ _
______
```
分割线效果图
![分割线效果图](MD%E5%AD%A6%E4%B9%A0.assets/163453809239799.png)

## 五、列表 ##
### 1.无序列表
```
//形式一
+ a
+ b
+ c
//形式二
- d
- e
- f
//形式三
* g
* h
* i 
```
列表展示图片
![列表展示图片](MD%E5%AD%A6%E4%B9%A0.assets/325070817247129.png)
### 2.有序列表
```
//正常形式
1. abc
2. bcd
3. cde
//错序效果
2. fgh
3. ghi
5. hij
```
有序列表效果图
![有序列表效果图](MD%E5%AD%A6%E4%B9%A0.assets/418242717239798.png)

> 如图，注意，数字后面的点只能是英文的点，有序列表的序号是根据第一行列表的数字顺序来的，错序列表的序号本来是序号是乱的， 但是还是显示 4 5 6
### 3.嵌套列表
```
//无序列表嵌套
+ 123
    + abc
    + bcd
    + cde
+ 465
+ 789
//有序列表嵌套
1. abcd
    1. abcde
    2. abcde
    3. abcde
2. bcde
3. cdef
```
嵌套列表效果图
![嵌套列表效果图](MD%E5%AD%A6%E4%B9%A0.assets/307282817236353.png)

> 列表可以嵌套，使用时在嵌套列表前按 tab 或 空格 来缩进,去控制列表的层数
## 六、表格
1. 表格不一定要对的非常整齐，但是为了编程的规范性，尽量对齐更好
2. 分割线后面的冒号表示对齐方式，写在左边表示左对齐，右边为右对齐，两边都写表示居中
```
//例子一
|123|234|345|
|:-|:-:|-:|
|abc|bcd|cde|
|abc|bcd|cde|
|abc|bcd|cde|
//例子二
|123|234|345|
|:---|:---:|---:|
|abc|bcd|cde|
|abc|bcd|cde|
|abc|bcd|cde|
//例子三
123|234|345
:-|:-:|-:
abc|bcd|cde
abc|bcd|cde
abc|bcd|cde
```
表格效果图
![表格效果图](MD%E5%AD%A6%E4%B9%A0.assets/406514009247592.png)

## 七、代码块
### 1.少量代码，单行使用，直接用`包裹起来就行了
```
` shaoliangdaima,danhangshiyong `
```
少量代码效果图
![少量代码效果图](MD%E5%AD%A6%E4%B9%A0.assets/98253609220671.png)


### 2.大量代码，需要多行使用，用```包裹起来,**注意换行**

    ```  
        daliangdaima,xuyaoduohangshiyong
        daliangdaima,xuyaoduohangshiyong
        daliangdaima,xuyaoduohangshiyong
        daliangdaima,xuyaoduohangshiyong
        daliangdaima,xuyaoduohangshiyong
    ```
大量代码效果图
![大量代码效果图](MD%E5%AD%A6%E4%B9%A0.assets/328283609239097.png)
## 八、引用说明区块
对某个部分做的内容做一些说明或者引用某某的话等，可以用这个语法。
### 1.正常形式
```
> 引用内容、说明内容。在语句前面加一个 > ，注意是英文的那个右尖括号，注意空格，引用因为是一个区块，理论上是应该什么内容都可以放，比如说：标题，列表，引用等等。
```
引用说明区块正常形式效果图
![引用说明区块正常形式效果图](MD%E5%AD%A6%E4%B9%A0.assets/204892917232107.png)
### 2.嵌套区块
给区块的下一级区块多加一个右尖括号
```
> 一级引用
>> 二级引用
>>> 三级引用
>>>> 四级引用
>>>>> 五级引用
>>>>>> 六级引用
```
嵌套区块效果图
![嵌套区块效果图](MD%E5%AD%A6%E4%B9%A0.assets/476292917249987.png)

## 九、链接
### 1.行内式
链接的文字放在[]中，链接地址放在随后的()中，链接也可以带title属性，链接地址后面空一格，然后用引号引起来
```
[简书](https://www.jianshu.com "创作你的创作"),
是一个创作社区,任何人均可以在其上进行创作。用户在简书上面可以方便的创作自己的作品,互相交流。 
```
[简书](https://www.jianshu.com "创作你的创作")

### 2.参数式

链接的文字放在[]中，链接地址放在随后的:后，链接地址后面空一格，然后用引号引起来

[简书]: https://www.jianshu.com "创作你的创作"

```
[简书]: https://www.jianshu.com "创作你的创作"
[简书]是一个创作社区,任何人均可以在其上进行创作。用户在简书上面可以方便的创作自己的作品,互相交流。
//参数定义的其他写法
[简书]: https://www.jianshu.com "创作你的创作"
[简书]: https://www.jianshu.com "创作你的创作"
[简书]: <https://www.jianshu.com> "创作你的创作"
```
### 3.行内式和参数式效果图一致
![链接效果图](MD%E5%AD%A6%E4%B9%A0.assets/45693709226964.png)

## 十、图片
### 1.行内式
和链接的形式差不多，图片的名字放在[]中，图片地址放在随后的()中，title属性（图片地址后面空一格，然后用引号引起来）,**注意的是[]前要加上!**

![my-logo.png](https://upload-images.jianshu.io/upload_images/13623636-6d878e3d3ef63825.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240 "my-logo")

```
![my-logo.png](https://upload-images.jianshu.io/upload_images/13623636-6d878e3d3ef63825.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240 "my-logo")
```
### 2.参数式
图片的文字放在[]中，图片地址放在随后的:后，title属性（图片地址后面空一格，然后用引号引起来）,**注意引用图片的时候在[]前要加上!**
```
[my-logo.png]: https://upload-images.jianshu.io/upload_images/13623636-6d878e3d3ef63825.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240 "my-logo"
![my-logo.png]
//参数定义的其他写法
[my-logo.png]: https://upload-images.jianshu.io/upload_images/13623636-6d878e3d3ef63825.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240 "my-logo"
[my-logo.png]: https://upload-images.jianshu.io/upload_images/13623636-6d878e3d3ef63825.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240 "my-logo"
[my-logo.png]: <https://upload-images.jianshu.io/upload_images/13623636-6d878e3d3ef63825.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240> "my-logo"
```
### 3.行内式和参数式效果图一致
![图片效果图](MD%E5%AD%A6%E4%B9%A0.assets/481433709247130.png)