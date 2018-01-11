# Danmu2Ass —— 弹幕xml/json文件转Ass字幕文件

## 介绍

Danmu2Ass是一款简单地将你的xml/json弹幕文件转换为ASS字幕文件的小工具。支持命令行和一些简单的开关。
此工具基于.NET Framework 4.0开发，转换核心基于Niconvert项目，运行环境为内置的IronPython 2.7。

## 下载

Danmu2Ass基于.NET Framework 4.0，如果您不是Win8用户，请[点此下载安装](http://www.microsoft.com/zh-cn/download/details.aspx?id=17718)后再使用本工具。

* **最新版本可以[在这里](https://danmu2ass.codeplex.com/releases)下载**

如果出现打不开等现象，请先暂时关闭您的360杀毒软件。

## 使用方式

1. **一般向**  
直接双击exe就能看到使用方法，会出现以下提示：
使用方法任选其一:
第一种-> 右键单击需要转换的xml/json弹幕文件，选择【发送到-转换为ASS字幕文件】
第二种-> 将需要转换的xml/json弹幕文件拖放到此程序的图标上
转换后的ASS文件将被放到原弹幕文件的旁边

2. **高手向**  
请运行 Danmu2Ass.exe -help 查看帮助。我也好心地贴在了下面
Danmu2Ass.exe [-help|/?] [-width XXX] [-height XXX] [-line XXX] [-bottom XXX]
[-shift XXX.XXX] [-S] File1 [File2,File3...]

    -help或/? 显示此提示  
    -width XXX 设置视频宽度为XXX，默认为1920  
    -height XXX 设置视频高度为XXX，默认为1080  
    -bottom X 设置为底部保留X分之一的区域，默认为6  
    -shift XXX.XXX 设置弹幕晚出现X秒，默认为0  
    -S 静默模式，程序完成时自动退出  
    File 文件完整路径，多个文件用空格隔开，包含空格的路径使用双引号括起来  

## 转换核心

转换核心使用[Niconvert](https://github.com/muzuiget/niconvert)项目的代码。  
此项目针对Niconvert项目做了一些必要的改动，包括将其运行环境从CPython向IronPython移植，精简不需要的代码，内联一些标准Python库代码，并增加了必要的互操作入口等。  
具体修改信息参见源代码中 /PythonFile/Niconvert.py 文件

## 开源协议

此项目使用GPLv2协议开源

## 联系作者

请发送邮件到 kaedei#foxmail.com (#替换为@)

## 以下是作者最新博客内容，欢迎来看看：

 Kaedei 的个人博客 News Feed  
[[初学者版]反编译apk方法](http://blog.sina.com.cn/s/blog_58c506600102x5gn.html)  
2017年8月14日  |  From [Kaedei 的个人博客](http://blog.sina.com.cn/rss/1489307232.xml)  
[近况](http://blog.sina.com.cn/s/blog_58c506600102x5d1.html)  
2017年8月12日  |  From [Kaedei 的个人博客](http://blog.sina.com.cn/rss/1489307232.xml)  
[三分钟让你的展会活动加上弹幕](http://blog.sina.com.cn/s/blog_58c506600102wybr.html)  
2017年2月19日  |  From [Kaedei 的个人博客](http://blog.sina.com.cn/rss/1489307232.xml)  
[截止2017/1/28还有效的AcFun弹幕解析方式](http://blog.sina.com.cn/s/blog_58c506600102wxcy.html)  
2017年1月28日  |  From [Kaedei 的个人博客](http://blog.sina.com.cn/rss/1489307232.xml)  
[弹弹play UWP版](http://blog.sina.com.cn/s/blog_58c506600102wvmy.html)  
2016年12月21日  |  From [Kaedei 的个人博客](http://blog.sina.com.cn/rss/1489307232.xml)  
[弹弹play“远程访问”功能API](http://blog.sina.com.cn/s/blog_58c506600102wv6o.html)  
2016年12月9日  |  From [Kaedei 的个人博客](http://blog.sina.com.cn/rss/1489307232.xml)  
[弹弹play“远程访问”功能应用列表](http://blog.sina.com.cn/s/blog_58c506600102wv6n.html)  
2016年12月9日  |  From [Kaedei 的个人博客](http://blog.sina.com.cn/rss/1489307232.xml)  
[VS2015中无法启动Xamarin Android调试怎么办？](http://blog.sina.com.cn/s/blog_58c506600102wk2t.html)  
2016年6月10日  |  From [Kaedei 的个人博客](http://blog.sina.com.cn/rss/1489307232.xml)  
[弹弹play5.5更新日志](http://blog.sina.com.cn/s/blog_58c506600102whmo.html)  
2016年5月3日  |  From [Kaedei 的个人博客](http://blog.sina.com.cn/rss/1489307232.xml)  
[教程：如何手动安装Xamarin系列](http://blog.sina.com.cn/s/blog_58c506600102wfy7.html)  
2016年4月13日  |  From [Kaedei 的个人博客](http://blog.sina.com.cn/rss/1489307232.xml)  
 Kaedei 的个人博客 News Feed  
Last edited Aug 15, 2013 at 12:11 PM by [kaedei](https://www.codeplex.com/site/users/view/kaedei), version 4
