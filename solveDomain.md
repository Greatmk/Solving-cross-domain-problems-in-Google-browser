#### 今天分享一下在开发中遇到的，谷歌浏览器如何跨域的方法（开发中最常见的解决办法）
````

这方法是投机取巧的方法，非常好用，希望总结一下可以帮到你！

1.windows系统如何解决谷歌浏览器跨域： 方法如下：

首先： 在桌面上选中谷歌浏览器，然后右键选择属性打开，然后找到快捷方式 下面的目标那一块，把“--disable-web-security --user-data-dir”这个双引号里面

的复制直接粘贴到 目标 哪一块的最后面，注意复制的时候有空格，最后点击应用和确定，然后把谷歌浏览器关掉，重新打开，在浏览器的地址栏那里出现一段淡黄色的一段

文字“您使用的是不受支持的命令行标记。。。。。”就代表你跨域成功了！！！


2.mac系统如何解决谷歌浏览器跨域： 方法如下：

首先：在你的mac电脑最左下角点击“Finder”并打开，然后点击“文稿”，在里面创建一个文件夹“MyChromeDevUserData”，接下来打开命令行，直接把“open -n 

/Applications/Google\ Chrome.app/ --args --disable-web-security  --user-data-dir=/Users/Great/Documents/MyChromeDevUserData ”

这双引号里面的复制粘贴到命令行，注意这里“/Users/Great/Documents/MyChromeDevUserData”的Great，是你Mac电脑的主机名，需要更改成你自己的Mac名子，

最后回车，mac电脑就自动打开谷歌浏览器并跨域了！！！！

```