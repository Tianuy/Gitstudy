# Markdown learning
想学markdown很有久了，今天终于是打算把它学习了，先学完这个，后面的再说吧，不能永远停留在计划上不是吗。
##  markdown 标题语法
#### 标题在文字前加#号

可选语法
=======
可选语法
-------

#### 可以在文本下添加任意数量的==号来标记一级标题，用任意数量的--号来标记二级标题
#### 不标记的行需要用空行隔开，不然会标记符号上面的所有的行。


###### 需要注意的是不同markdown应用程序处理 # 和标题之间的空格方式是不同的，为了兼容请用一个空格将两者隔开。

## 段落语法
##### 要创建段落，请使用空白行或多行对文本进行分割，不要像语文里一样使用空格space或者制表符tabs缩进段落。
  
  
换行语法
-------
#### 在一行的末尾添加两个或多个空格，然后按回车键，即可创建一个换行<br>    
##### 几乎每个 Markdown 应用程序都支持两个或多个空格进行黄行，被称为 ## 结尾空格 trailing whitespace ，但这是有争议的，因为很难在编辑器中直接看到空格，并且很多人在每个句子后面都会有意或无意地添加两个空格。由于这个原因，得需要其他的方式进行换行，几乎每一种Markdown的应用程序都支持另一种换行方式： ## HTMLL 的 <br> 标签。

aklfdjlashfaj<br>adjflajfalfj

##### 还有两种不推荐的方式，但应用程序很少，在末尾加\和直接加return键<br>


## Markdown 强调语法  
### 粗体Bold  
#### 要加粗文本需要在文本前后加两个asterisks星号**或两个underscores下划线 _ .如需加粗一个单词中间的部分，要两侧各加上两个星号asterisks  
**bold**  __bold__ bold
##### Markdown应用程序在如何处理单词或短语中间的下划线上并不一致，为了兼容，在单词或短语中间部分加粗时，用星号asterisks  
### 斜体  ltalic
#### 要用斜体显示文本，在文本前后添加一个星号asterisks 或下划线 underscores，前显示单词中的，前后添加一个星号，中间不要带空格。
*star*  _star_ star
##### 同时需要加粗斜体时 ，在需要突出部分前后各添加三个星号或下划线，中间不要带空格. 单词中的用星号  


## Markdown 引用语法  
### 要创建块引用，请在段落前添加一个>符号  
> www.baidu.com  
> reworuqr\
> kdal**hal**lsjf  

### 多个段落的块引用，块引用可以包含多个段落，为段落之间的空白行添加一个>符号  
> www.baidu.com
> www.xvdieos.com
>
> www.google.com

### 嵌套块引用， 块引用可以嵌套，在要嵌套的段落前添加一个>>符号  
>www.baidu.com  
>>the witch bade her claen the pots 

### 带有其他元素的块引用 ，块引用可以包含其他Markdown格式的元素，并非所有元素都可以使用，需要进行实验以查看哪些元素有效  

## Markdown 列表语法  
### 有序列表 要创建有序列表，请在每个列表项前添加数字并紧跟一个英文句点。数字不必按数字顺序排序，但是列表应当以数字1开始  
1. First item
2. second item
   1. lidented item
3. Third item

**部分程序支持用)代替.但是只是部分而已**  
1) first item
2) second item
   1) lidented item
3) third item  
     
### 无序列表 要创建无序列表请在每个列表项前添加破折号- 星号* 或加号  
* First item
* Second item
  * lidented item
* Third item

- First item
- Second item
  - lidented item  
- Third item
  
+ First item
+ Second item 
  + lidented item
+ Third item 

### 在列表中嵌套其他元素 
#### 要在保留列表连续性的同时在列表中添加另一种元素，请将该元素缩进四个空格或一个制表符  
* First item
    >www.baidu.com
* Second item
* Third item
#代码块通常采用四个空格或一个制表符缩进，当把他们放在列表中时，请将他们缩进八个空格或两个制表符
1. Open the file 
2. Find the following code block on line 21:
        &lt;html>  
        &lt;head>
        &lt;tittle>Test&lt;/title>
3. Update the title to   

## Markdown 代码语法  
#### 要将单词或短语表示为代码，请将其包裹在反引号`中  

`int main(void)`
#### 转义反引号 如果代码中包含反引号，则将代码包裹在双反引号中
``#inclu`de<stdio.h>``  
#### 围栏代码块 Markdown基本语法允许将行缩进四个空格或一个制表符来创建代码块。
    #include<stdio.h>  
    int main(void)
    {
        int i,j;
        `printf("Hello world!")\n;
        return 0;
    }

如果发现不方便可以使用受保护的代码块。在代码块之前和之后的行上使用三个反引号```或三个波浪号~~~  
```
#include "stdio.h"
int main (void)
{
    int i,j;
    printf("hello world!")\n;
    return 0;
}
```
#### 语法高亮 
##### 许多Markdown处理器都支持受围栏代码块的语法突出显示。使用此功能，可以为编写代码的任何语言添加颜色突出显示。添加语法突出显示在受保护的代码块之前的反引号旁边指定一种语言。
```c
#include "stdio.h"
int main (void)
{
    int i,j;
    printf("hello world!")\n;
    return 0;
}
```
### Markdown分隔线语法  
要创建分隔线，请在单独一行上使用三个或多个星号***，破折号---或下划线，并且不能包含其他内容  
***
---
___
为了兼容性，在分隔线的前后均添加空白行  
  
---

### Markdown链接语法  
链接文本放在中括号内，链接地址放在后面的括号中，链接title可选。  title和地址之间以空格隔开。
**超链接Markdown语法代码**[超链接显示名](超链接地址"超链接title")
[这是一个链接](https://markdown.com.cn "最好的markd教程")

#### 网址和Email地址
使用尖括号可以很方便地把URL或者email地址变成可点击的链接  
<tianyuyasin@outlook.com>
<https://markdown.com.cn>

[最好的markdown教程](https://markdown.com.cn "最好的markdown教程")
#### 带格式化的链接  
**强调**链接，在链接语法前后增加星号，要将链接表示为代码，请在方括号中加反引号。
I love the **[apple](https://www.apple.com.cn "apple")**  
i love the *[apple](https://www.apple.com.cn "apple")*  
i love the [`code`](https://www.apple.com.cn)
#### 引用类型链接
引用样式链接是一种特殊的链接类型,它使URL在Markdown中更易于显示和阅读。参考样式链接分为两个部分：与文本保持内联的部分以及储存在文件中其他位置的部分，以让文本易于阅读

##### 链接的第一部分格式
引用类型的链接的第一部分使用两组括号进行格式设置。第一组方括号显示为链接的文本，第二组括号显示一个标签，该标签用于指向储存在文档其他位置的链接
 
尽管不是必需的，可以在第一组和第二组括号之间包含一个空格，第二组括号中的标签不区分大小写。

[apple] [1]
##### 链接的第二部分格式
引用类型链接的第二部分使用以下属性设置格式： 

1. 放在括号中的标签，其后紧跟一个冒号至少一个空格  
2. 链接的URL，可以选择将其放在尖括号中。  
1. 链接的可选标题，可以将其放在双引号或括号中. 

[apple] [2]
[apple] [3]

[1]: <https://www.apple.com.cn> 
[2]: <https://www.baidu.com> 
[3]: <https://1drv.ms/b/c/39435707fad57e89/EYl-1foHV0MggDliKAAAAAABpunJn0-Elp-UKQsbiQI0dg?e=J8t7e9> 

**可以将链接的第二部分放在Markdown文档中的任何位置。**
##### 链接最佳实践  
不同的Markdown应用程序处理URL中间的空格方式不一样，为了兼容性，用%20代替空格

[link](https://www.example.com/my%20great%20page)  
### Markdown 图片语法  
要添加图片，请使用感叹号！，然后在方括号增加代替文本，图片的链接放在圆括号中，括号的链接后可以增加一个可选的图片标题文本<br>
![这是我宝贝](img/1.jpg "BB")
#### 链接图片
要给图片增加链接，使用链接的方法即可，将图像的markdown括在方括号中，然后将链接加的圆括号中
[![这是我宝贝](img/.jpg "宝贝")](https://www.apple.com.cn)  

### Markdown转义字符语法  
要显示原本用于格式化Markdown文档的字符，请在字符前面添加反斜杠字符\  
\* Without the backslash*<br>
* without the backslash
#### 可做转义的字符  
一下列出的字符都可以通过反斜杠字符从而达到转义的目的
\
`
*
_
{}
[]
()
#
+
-
.
!
|

#### 特殊字符自动转义
在HTML文件文件中，有两个字符需要特殊处理: < 和 & ，< 符号用于起始标签，&符号则用于标记HTML实体，如果你只是想要使用这些符号，你必须要使用实体的形式的形式，像是&lt 和 &amp；
&符号其实很容易让写网页文件的人感到困扰，如果你要打[AT&T],你必须要写成[AT&amp;T],还得转换网址内的&符号，如果你要链接到：
http://images.google.com/images?num=30&q=larry+bird
必须转换到
http://images.google.com/images?num=30&amp;q=larry+bird  

Markdown允许你直接使用这些符号，它帮你自动转义字符。如果你使用&符号作为HTML实体的一部分，那么它不会被转换，而且其他情况下，它则会被转换成&amp；。所以如果要在文件中插入一个著作权的符号，你可以这样写：
&copy；<br>
Markdown不会对这段文字做修改，但是如果你这样写：
AT&T;
AT&amp;T
4<5
4 < 5
4 &lt; 5

Markdown的块级元素和内联元素中，< 和 &两个符号会被自动转换成HTML实体，这项特性让你可以很容易地用Markdown写HTML。
