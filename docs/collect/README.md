# 神器收藏

## 代码截图
* [一键生成代码截图](https://quanxin.org/code-snapshot)

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
* win10 开启开启卓越性能电源方案（需要PowerShell管理员）
> ``powercfg -duplicatescheme e9a42b02-d5df-448d-aa00-03f14749eb61``

### Windows 下播放器
> 主要参考：https://www.v2ex.com/t/951012#reply176
- [potplayer](https://potplayer.daum.net/) UI完整，使用简洁，功能全面
  > 黑历史：使用了ffmpeg开源代码，然而不遵循开源协议
  > 新版有广告，并且会上报播放记录等隐私

  - [禁止 PotPlayer 广告、发送数据(WINDOWS 11)](https://go123.live/blocking-connection-from-potplayer-in-windows-firewall/)
  - [PotPlayer + LAV Filters + XySubFilter + MadVR配置指南](https://blog.csdn.net/sigmarising/article/details/105700625)
  - [K-Lite Codec Pack](https://codecguide.com/download_k-lite_codec_pack_mega.htm)
- [mpv](https://mpv.io/installation/) 功能强大，可繁可简，高度可配置文件(还有mac版) 
  > [mpv + uosc极简UI](https://github.com/tomasklaen/uosc)
- [mpc-hc](https://github.com/clsid2/mpc-hc) 开源，其他作者基于停更后的mpc继续维护的 
- [mpc-be](https://github.com/Aleksoid1978/MPC-BE) mpc原作者之一出走后维护的项目

## macOS
* [Awesome Mac](https://wangchujiang.com/awesome-mac/index.zh.html)
* [从 Windows 到 macOS - Sherlock - 个人博客](https://halo.sherlocky.com/archives/macos)

## Office
* [PDF转PowerPoint](https://www.pdfpai.com/pdf-to-powerpoint)

## Crack
* [常用破解软件](https://www.fxxkmakeding.xyz/downloads.html)
> [github版地址](https://github.com/xyjoey/fxxkmakeding)

## 颜值即正义
* [那些管UI小姐姐要来的网站](https://juejin.im/post/5e7cdee26fb9a03c6e640cc7)

## 在线自动拼图
- 常见资源大图获取方法(https://new.shuge.org/download_zoomable_images/)
 > 例如可获取故宫博物院数字藏品高清图片
 > [九成宫醴泉铭-宋拓本](https://www.dpm.org.cn/collection/impres/234127.html)
- [使用开源项目：dezoomify](https://ok.daoing.com/he/dezoomify.html)
