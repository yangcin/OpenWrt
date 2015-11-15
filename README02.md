#安装配置 shadowsocks-libev
Shadowsocks并不在Openwrt官方软件源里，因此需要下载.ipk文件自行安装。<br>
Shadowsocks有众多版本，这里采用 [aa65535](http://sourceforge.net/u/aa65535/profile/) 编译的版本。
####下载软件
- [ShadowSocks-libev-PolarSSL](http://sourceforge.net/projects/openwrt-dist/files/shadowsocks-libev/) 最新版为 2.4.1-6f44d53 （2015-11-16）

####安装ipset
	opkg update
	opkg install iptables-mod-nat-extra ipset libpolarssl
####卸载dnsmasq并安装dnsmasq-full
	opkg remove dnsmasq && opkg install dnsmasq-full
####安装shadowsocks-libev
	cd /tmp
	opkg install shadowsocks-libev-polarssl_2.4.1-1_ar71xx.ipk
####配置软件
  	mkdir /etc/dnsmasq.d
  	echo "conf-dir=/etc/dnsmasq.d" >> /etc/dnsmasq.conf
