# Ubuntu 16.04 PHP-Redis扩展
# 流程

1.安装PHP-dev

`sudo apt-get install php7.0-dev`

2.PCEL编译redis扩展

`sudo pecl install redis`

3.PHP扩展手动添加扩展

`/etc/php/7.0/fpm/conf.d  扩展目录`

创建新的扩展文件redis.ini  <br>

`extension=redis.so`

4.重启生效

`sudo service php7.0-fpm restart`