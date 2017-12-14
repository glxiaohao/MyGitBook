# Introduction
welcome to guoling bookHouse 
ctrl + alt + v （先用QQ剪切想要的图片）拷贝图片到md文件
```
glxiaohao
glxiaohao_123
http://gl.yystudying.com:4000/chapter6/redis/redis.html
```

![](git.png)

cd /root/code/MyGitBook/gitbookProject/bookHouse
git pull origin master

### 效果图
![](git_pull.png)

### github查看网址
https://github.com/

导出python_gl数据库里的所有表及表数据到1.sql(注意在1.sql所在的目录下，不需要登录mysql)
mysql -uroot -p python_gl > 1.sql;

方式一：
导入数据到bak
create database bak charset utf8;
use bak;
source 1.sql

方式二：
create database bak charset utf8;
exit
mysql -uroot -p bak < 1.sql;

