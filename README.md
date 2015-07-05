#NginX Mirroring
##简介

只利用NginX实现的镜像服务器，可用于加速访问速度较慢的源

##安装方法

以Ubuntu 14.04为例

1. 安装nginx服务器，apt-get install nginx

2. 复制nginx/mirror.malash.net到nginx vhost目录，一般为/etc/nginx/sites-available/，并在/etc/nginx/sites-enabled/建立软链接

3. 修改/etc/nginx/sites-available//mirror.malash.net中的域名，建议使用全局替换“mirror.malash.net”为新域名

4. 复制www内的文件到合适的位置，并修改/etc/nginx/sites-available//mirror.malash.net中root值

##使用方法

主镜像地址：
```
http://downloads.openwrt.org/
```
Mirror地址：
```
http://downloads.openwrt.org.mirror.malash.net/
```
或
```
http://mirror.malash.net/downloads.openwrt.org/
```
