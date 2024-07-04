# 玩儿

* [如何把自己的Jar包上传到 maven 官方仓库中，Maven上传图文讲解](https://www.sojson.com/blog/250.html)
* [发布Maven构件到中央仓库](https://www.xncoding.com/2018/01/27/tool/maven-central.html)
* [使用Gradle发布构件(Jar)到Maven中央仓库](https://segmentfault.com/a/1190000018026290)
* [Gradle 发布 JAR 包到 maven 中央仓库(sonatype )](https://blog.csdn.net/mr_zhuqiang/article/details/84564256)

## 数据无价
* [3-2-1 备份策略](https://www.backblaze.com/blog/the-3-2-1-backup-strategy/)

## NAS 
* [群晖 NAS 之 Docker Nginx 反向代理](https://halo.sherlocky.com/archives/nas-docker-nginx)
* [群晖 NAS 下 CentOS7 虚拟机挂载主机磁盘](https://halo.sherlocky.com/archives/qun-hui-nas-xu-ni-ji-gua-zai-zhu-ji-ci-pan)
* [群晖 NAS Docker 容器镜像加速](https://halo.sherlocky.com/archives/qun-hui-nas-docker-rong-qi-jing-xiang-jia-su)
* [使用 Rocky Linux 打造家用 NAS 系统](https://rockylinux.cn/notes/strong-shi-yong-rocky-linux-da-zao-jia-yong-nas-xi-tong.html)

## 博客
* [~~给自己博客添加 Elasticsearch 实现全文搜索~~](https://halo.sherlocky.com/archives/docker-es)
  > halo 2.X+ 已支持全文搜索
* [CentOS7 Certbot 自动更新 Let's Encrypt SSL 证书(Nginx,https)](https://halo.sherlocky.com/archives/centos7-certbot-nginx-ssl)

## 家庭影院

### 回音壁
* [什么是音频回传(ARC)功能？](https://www.sony.com/zh-cn/electronics/support/articles/00012943?showHeaderFooter=false)
  > eARC（Enhanced Audio Return Channel）是ARC的加强版，是由HDMI 2.1标准化的新功能，除了支持现有ARC（Audio Return Channel）所支持的音频格式，还支持最新的音频格式。
  > 使用HDMI线缆连接系统和兼容eARC的电视机，即可欣赏无法用ARC传输的Dolby Atmos - Dolby TrueHD和DTS:X等对象音频内容，或多声道LPCM内容。
  > 
  > 如回音壁与电视机均支持ARC功能，将回音壁与电视机连接时，ARC功能可以免去使用额外复合音频线或光纤线缆的必要。  
  >
  > 使用HDMI®线缆将兼容ARC的回音壁与兼容ARC的电视机连接，可以实现以下操作：
  > 
  > - 1、将音频从电视机发送到回音壁。
  > - 2、观看和收听来自源设备（例如：蓝光播放机）的电影和其他内容，其视频画面信号可通过回音壁在电视上播放。 
  > 
  > 使用支持ARC的HDMI 线连接电视机与音频设备的HDMI ARC端口。
  > 
  > NOTE: 没有贴符高速度的低质量HDMI是没有ARC功能的。
  > 
  > ![image](https://github.com/sherlocky/learning/assets/8652013/bc6be903-abb1-4934-8ace-3cb10e6adf99)
  > 
  > - A: TV
  > - B: 音频设备
  > - C: 电视HDMI ARC 输入端口
  > - D: 音频设备HDMI ARC 输出端口
  > - E: 支持ARC的HDMI 线(高质量，高速度的HDMI线)
* 哪些情况/场景之下需要用到 eARC/ARC？
  > 其实只是需要由电视经 HDMI 输出音效，都会用到 eARC/ARC。
  > 
  > - 而其中一个常见情况是：电视配搭 Soundbar 提升音效，不过 Soundbar 只设有一组 HDMI（eARC/ARC）接口，就需要通过 HDMI 连接电视回传声效到 Soundbar 输出；
  > - 另一个情况是：Soundbar 的 HDMI 接口不足够连接额外的 Apple TV、Now E 机顶盒、PS5、XBOX 等器材，就可以通过 HDMI 连接电视，再将音效回传到 Soundbar。
  > - 还有一种特殊情况：【电视不支持 eARC的情形】使用 HDMI 连接播放机的 HDMI OUT端口和Sound Bar的HDMI IN 端口 + 使用 HDMI 线缆连接Sound Bar的HDMI OUT eARC/ARC 端口和电视 HDMI IN端口。
  >   这种是比较特殊的用法。

* eARC要求
  > 首先电视和通过 HDMI 连接的音效输出器材（e.g. Soundbar、AV 功放、两声道功放、主动式音箱等）都要同时兼容 eARC 或者 ARC。
  > 另外在设置上有机会要手动启用 eARC/ARC，以及 HDMI CEC（消费者电子控制、Consumer Eletronics Control）等相关功能。
  > 
  > 基本上具备 Ethernet 网络功能的标准或者 High-Speed HDMI 线部分可以用作回传音讯，而 Ultra High-Speed HDMI 就一定支持。
  > 连接方面要留意，电视只有一个 HDMI 接口支持 eARC/ARC，Soundbar 和 AV 功放等音效输出器材也是同样只有一组支持，HDMI 线要连接到支持 eARC/ARC 的接口才可以使用音效回传功能。
  
* [如何使用Sound Bar播放Dolby Atmos格式的音频](https://www.sony.com/zh-cn/electronics/support/sound-bars-home-theater-systems-sound-bars-surround-speakers/ht-a5000/articles/00194917)
  > 连接到与 HDMI 兼容的电视 （eARC)  
  >
  > 当Sound Bar连接到HDMI（eARC/ARC）端口时，您可以播放以下内容：
  > 
  > - 电视播放的Dolby Atmos格式的内容
  > - 从播放设备（如蓝光光盘播放器）播放的Dolby Atmos格式内容  
  >
  > 连接方式：
  > 
  > - 使用 HDMI 线缆（D）连接 Sound Bar的HDMI OUT eARC/ARC 端口和电视的 HDMI IN eARC/ARC端口。
  > - 使用 HDMI 线缆（E）连接播放设备的 HDMI 输出端口和电视或Sound Bar的HDMI IN 端口。
  > 注意： 您可以将HDMI 线缆(E) 连接到Sound Bar的 HDMI IN 端口或者电视的 HDMI IN 端口, 但请注意不要同时连接两个端口。
  > ![image](https://github.com/sherlocky/learning/assets/8652013/b0f9ee23-49b4-41e4-828e-0b04f07f0c99)
  >
  > - A: Sound Bar
  > - B: 电视
  > - C: 蓝光光盘播放器
  > - D: HDMI电缆（支持以太网）
  > - E: HDMI 电缆
* [如何将电视机与Sound Bar建立连接？](https://www.sony.com/zh-cn/electronics/support/sound-bars-home-theater-systems-sound-bars-surround-speakers/ht-a5000/articles/00014997)
  - 1、如果电视机的HDMI接口支持ARC
    > 如果是连接到比较新的电视机即HDMI接口支持ARC功能，可以使用HDMI线连接电视机的HDMI （ARC）接口至Sound bar上的TV out ARC。
    >
    > ![image](https://github.com/sherlocky/learning/assets/8652013/2a17638d-5ebc-47f0-b0c8-ce171e2f3048)
    > 
    > - A: Sound Bar (背部)
    > - B: HDMI  (ARC)
    > - C: HDMI 线
    > 
    > 注意: 如果电视机的HDMI接口支持ARC，则会有ARC的标识，如果连接的HDMI 没有此标识，则就不支持ARC功能。
  - 2、如果电视机的HDMI接口不支持ARC但有光纤接口
    > 2.1 有些电视机型号有HDMI接口但不支持ARC功能，可以先使用HDMI线连接电视机的HDMI接口至Sound bar的TV out ARC接口，然后再使用光纤线连接电视机的光纤接口至Sound bar的Optical in接口（为了听到电视机的声音，此为必要步骤）。
    >
    > ![image](https://github.com/sherlocky/learning/assets/8652013/1d334db2-5c7a-45b7-9245-bdf7f9de6065)
    > 
    > - A: Sound Bar (背部)
    > - B: HDMI IN
    > - C: 光纤音频输出
    > - D: HDMI 线
    > - E: 光纤线
    > 
    > 2.2 如果电视机没有HDMI接口但有光纤接口 使用光纤线连接电视机的光纤接口至Sound bar的Optical in接口。
    >
    > ![image](https://github.com/sherlocky/learning/assets/8652013/29623985-54de-4148-b22f-bb4d321585e8)
    > 
    > - A: Sound Bar (背部)
    > - B: 光纤音频输出接口
    > - C: 光纤线
  - 3、如果电视机没有HDMI接口同时也没有光纤接口
    > 可以使用音频线连接电视机的音频输出至Soundbar的ANALOG IN 接口。
* [【视频】家庭影院入门2番外篇——回音壁实战（开箱、摆位、接线、调试、享受）](https://www.bilibili.com/video/BV1PG4y1f7hC/?p=4)
