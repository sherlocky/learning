# Audio & Video

## RTC
* [直录播常见误区](https://halo.sherlocky.com/archives/rtc)

## 音频
* [音频信号基础知识：波形、功率、强度、响度、音质](https://blog.csdn.net/rambo_csdn_123/article/details/119033157)
* [音频特征---波形图](https://blog.csdn.net/booklijian/article/details/106974667)
* [音频特征----频谱图](https://blog.csdn.net/booklijian/article/details/106979528)

## 字幕

* [爱幕-在线字幕制作](https://online.aimu-app.com/)
  > 时间轴、字幕、波形。。

### srt
格式示例（[示例下载](/static/demo.srt)）：
```bash
1
00:00:00,306 --> 00:00:00,844
那一天
あの日

2
00:00:01,280 --> 00:00:02,220
星星降落的日子
星が降った日

3
00:00:03,148 --> 00:00:04,412
那简直是
それはまるで
```

### ass(AdvancedSubStationAlpha)/ssa(SubStationAlpha)
格式示例（[示例下载](/static/demo.ass)）：
```
[Script Info]
; // 此字幕由爱幕生成
Synch Point:1
ScriptType:v4.00+
Collisions:Normal

[V4+ Styles]
Format: Name, Fontname, Fontsize, PrimaryColour, SecondaryColour, OutlineColour, BackColour, Bold, Italic, Underline, StrikeOut, ScaleX, ScaleY, Spacing, Angle, BorderStyle, Outline, Shadow, Alignment, MarginL, MarginR, MarginV, Encoding
Style: Default, Source Han Sans CN Normal, 20, &H00FFFFFF, &H000092FE, &H00000000, &H82000000, 0, 0, 0, 0, 100, 100, 0, 0, 1, 1, 2, 2, 10, 10, 30, 134
Style: Style1, Source Han Sans CN Normal, 20, &H0000DCFC, &H0000DCFC, &H00000000, &H82000000, 0, 0, 0, 0, 100, 100, 1, 0, 1, 1, 2, 2, 10, 10, 30, 134
Style: Style2, ZCOOL KuaiLe, 20, &H0000DDA4, &H0000DDA4, &H00334D19, &H82000000, 0, 0, 0, 0, 100, 100, 1, 0, 4, 1, 3, 2, 10, 10, 50, 134
Style: Style3, Source Han Sans CN Medium, 28, &H009E14AB, &H009E14AB, &H00009EFB, &H82000000, 0, 0, 0, 0, 100, 100, 1, 0, 1, 1, 2, 2, 10, 10, 100, 134

[Events]
Format: Layer, Start, End, Style, Actor, MarginL, MarginR, MarginV, Effect, Text
Dialogue: 0,0:00:00.31,0:00:00.84,Style1,NTP,0000,0000,0000,,那一天\N{\fs12}{\3c&&H00000000&}{\c&&H000092FE&}あの日
Dialogue: 0,0:00:01.28,0:00:02.22,Style2,NTP,0000,0000,0000,,星星降落的日子\N{\fs12}{\3c&&H00000000&}{\c&&H000092FE&}星が降った日
Dialogue: 0,0:00:03.15,0:00:04.41,Style3,NTP,0000,0000,0000,,那简直是\N{\fs12}{\3c&&H00000000&}{\c&&H000092FE&}それはまるで
Dialogue: 0,0:00:05.12,0:00:06.30,Default,NTP,0000,0000,0000,,像梦中的景色一样\N{\fs12}{\3c&&H00000000&}{\c&&H000092FE&}夢の景色のように
```
* 神器 Subtitle Edit

### H5 字幕``.vvt``
格式示例[示例下载](/static/demo.vtt)
```bash
WEBVTT

1
00:00:00.306 --> 00:00:00.844
那一天
あの日

2
00:00:01.280 --> 00:00:02.220
星星降落的日子
星が降った日

3
00:00:03.148 --> 00:00:04.412
那简直是
それはまるで
```

* HTML5 Video视频支持外挂字幕，文件后缀名是``.vtt``，称为 WebVTT (Web Video Text Tracks) 格式，专门的web字幕格式。
  > 使用很简单，用一个``<track>``元素即可，官方文档：https://w3c.github.io/webvtt/
  > CSS中有专门的伪元素``::cue``可以控制字幕的样式
* ``.vtt``文件的MIME type是``text/vtt``，在Chrome和safari浏览器下，是可以无障碍加载显示的。通常我们保存在电脑中的外挂字幕都不是 vtt 而是，常见的如 srt 格式。
* [WebVTT字幕格式](https://www.cnblogs.com/tocy/p/subtitle-format-webvtt.html)
* [SubRip to WebVTT converter](https://atelier.u-sub.net/srt2vtt/)
  > ``ffmpeg -i source.en.vtt target.en.srt``
