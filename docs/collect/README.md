# 神器收藏

## 代码比对
* [Linux 下 9 种优秀的代码比对工具推荐](https://mp.weixin.qq.com/s?__biz=MzAxODI5ODMwOA==&mid=2666546845&idx=2&sn=a8a638a300311344509770c1c3a8cd75)

## 画图
* [标准流程图符号和用法](https://www.edrawsoft.com/cn/flowchart-symbols.php)
* [draw.io画图工具](https://app.diagrams.net/)
* [ProcessOn在线画图工具](https://www.processon.com/)

## Windows
* [MSDN, 我告诉你 - 系统、Office下载](https://msdn.itellyou.cn/)
* [Microsoft Visual C++ 2015-2019 Redistributable](https://support.microsoft.com/en-us/help/2977003/the-latest-supported-visual-c-downloads)
* [Windows上优质&精选的最佳应用程序及工具列表](https://github.com/Awesome-Windows/Awesome/blob/master/README-cn.md)

* [win10 家庭版下载文件时没有权限保存到某盘的解决方案的完美流程](https://blog.csdn.net/weixin_42997646/article/details/89414437)
> win10 家庭版打开组策略方法（保存为.bat，管理员权限运行）

```
@echo off
pushd "%~dp0" 
dir /b C:\Windows\servicing\Packages\Microsoft-Windows-GroupPolicy-ClientExtensions-Package~3*.mum >List.txt 
dir /b C:\Windows\servicing\Packages\Microsoft-Windows-GroupPolicy-ClientTools-Package~3*.mum >>List.txt 
for /f %%i in ('findstr /i . List.txt 2^>nul') do dism /online /norestart /add-package:"C:\Windows\servicing\Packages\%%i" 
pause
```

## Office
* [PDF转PowerPoint](https://www.pdfpai.com/pdf-to-powerpoint)

## Crack
* [常用破解软件](https://www.fxxkmakeding.xyz/downloads.html)
> [github版地址](https://github.com/xyjoey/fxxkmakeding)

## 颜值即正义
* [那些管UI小姐姐要来的网站](https://juejin.im/post/5e7cdee26fb9a03c6e640cc7)
