# MyCodeSnippets
一、什么是代码片段

当在Xcode中输入dowhile并回车后，Xcode会出现下图所示的提示代码：

![](http://img.blog.csdn.net/20130929180431781?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvd3p6dmljdG9yeQ==/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)

这就是代码片段，目的是使程序员以最快的速度输入常用的代码片段，提高编程效率。该功能是从Xcode4开始引入的。在Xcode中的位置如下图所示：

![](http://img.blog.csdn.net/20130929181841921?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvd3p6dmljdG9yeQ==/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)

里面有很多Xcode自带的代码片段，上例中的dowhile就是其中的一个。

二、如何自定义代码片段

由于项目、所用语言或者编码习惯的差别，不同的程序员习惯用的代码片段也不尽相同，这就有了自定义代码片段的需求，好在Xcode是支持该功能的。

@property属性的定义是Cocoa程序开发中很常用的一个功能，下面就以此为例说明如何自定义代码片段。

1、书写代码片段

在声明@property属性的地方写下如下语句：

**[cpp]** [view plain](http://blog.csdn.net/wzzvictory/article/details/12163939#)[copy](http://blog.csdn.net/wzzvictory/article/details/12163939#)

1. @property (nonatomic, retain) <#type#> <#name#>;  

这里<#type#>和<#name#>起什么作用可以在后面的使用效果中看出来。

2、新建代码片段

选中上述语句，用鼠标左键拖到上图中指示的代码片段在Xcode中的区域里，就新建了一个代码片段

3、编辑代码片段

经过第2步操作，松开鼠标左键的同时，会弹出代码片段编辑窗口，如下图所示：

![](http://img.blog.csdn.net/20130929182943812?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvd3p6dmljdG9yeQ==/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)

图中从上到下的含义依次是：

①Title

代码片段的标题

②Summary

代码片段的描述文字

③Platform

可以使用代码片段的平台，有IOS/OS X/All三个选项

④Language

可以在哪些语言中使用该代码片段

⑤Completion Shortcut

代码片段的快捷方式，比如本文开头用到的dowhile，在这里，把属性设置的快捷方式设为property

⑥Completion Scopes

可以在哪些文件中使用当前代码片段，比如全部位置，头文件中等，当然可以添加多个支持的位置。

最后的一个大得空白区域是对代码片段的效果预览。

一切设置完成以后，点击该菜单右下角的Done按钮，新建工作就结束了。

三、代码片段的使用

有两种方式使用我们自定义的代码片段，还是以刚定义的@property属性代码片段为例：

1、在适当的位置（因为定义代码片段的时候可以设置使用平台，使用语言，使用文件等限制条件），输入property

2、直接在代码片段部分找到我们刚定义的那个，用鼠标左键拖动该代码片段到合适的位置

使用上面的两种方法中的任何一个以后，可以看到下图所示的效果：

![](http://img.blog.csdn.net/20130929183935093?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvd3p6dmljdG9yeQ==/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)

这里，大家注意到在定义代码片段时书写的<#type#>和<#name#>所起到的作用了吧！

四、代码片段的备份

Xcode中的代码片段默认放在下面的目录中：

**[java]** [view plain](http://blog.csdn.net/wzzvictory/article/details/12163939#)[copy](http://blog.csdn.net/wzzvictory/article/details/12163939#)

1. ~/Library/Developer/Xcode/UserData/CodeSnippets   

我们可以将目录中的代码片段备份，也可以将其直接拷出来放在不同的电脑上使用，因此多台电脑之间的协作也毫无压力。


