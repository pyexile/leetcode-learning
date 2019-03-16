python3+django2实现一个作业管理平台
一. 基本要求
1. 环境及包
  python3.6
  pymysql  # 连接数据库
  requests  # 爬取音乐时所需要
  django==2.1.5
  shutil  # 文件操作的一个包，例如可以打包文件
  
二. 版本更新

2019/3/5更新

1. 将主要的业务逻辑代码放在了同名的helper.py下；
2. 作业名限制变少，即不一定要学号开头；利用正则表达式将数据库中的改作业的值改为1，比之前之前死板的用学号要更好；
3. 页面可以显示当前用户；
4. 不再限制用户在线时长；
5. 下载作业中文名的那儿，现在不再是用正则匹配，而是用file.name这样得到文件名，这样就不用担心匹配不到而出错了
6. 将static/images中的图片名改为了英文名，预防出错。
7. 更新了tm_uwsgi.ini和tm_nginx.conf配置文件的内容。
