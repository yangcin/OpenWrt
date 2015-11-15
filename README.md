#打造 OpenWrt 智能路由器的小白教程
高手请绕道！<br>
小白请细阅！
##选择什么样的路由器？
兲朝有万能的某宝，搜索关键词 openwrt 能跳出100+页的结果，并且便宜得一塌糊涂<br>
重要的是对照一下 [OpenWrt官方网站](https://openwrt.org/) 的 [设备支持列表](https://wiki.openwrt.org/toh/start)<br>
总而言之，我选择了小型化的AP型智能路由。<br>
为什么呢？<br>
我习惯到处走，不方便携带怎么行？
##刷什么版本的OpenWrt？
不二的选择：最新稳定版，不刷 Snapshot 版
- 最新稳定版 [Chaos Calmer 15.05](https://downloads.openwrt.org/chaos_calmer/15.05/)   发布于 2015-9-11 星期五

嘿，这日子，又适逢星期五还？我怎么会说“又”呢！
## OpenWrt 刷机方法
设置电脑本地连接为 192.168.1.2 255.255.255.0<br>
部分路由器如D-LINK等，需设为192.168.0.1，这些路由刷完openwrt后，需第二次改IP为192.168.1.1<br>
下载windows应用软件<br>
