### 本 Fork 更新:<br>

3/22<br>
1. 更新了文件中的描述 PHP 版本, 因为 heroku 现在不支持较低的 PHP 版本, 会导致部署错误.<br>
2. 去掉了密码验证, 方便观看.<br>
3. 更新了 config 设置. 请在 confing.php 文件中自定义网站名字, 以及参考官方文档设置自己的 API key, 当部署此 Fork 人数过多, API 配额用尽时网站将不可用.<br>


<b>YouTube 镜像网站, 实现免翻墙访问.</b><br>
点击使用: https://youtubemirror-usa.herokuapp.com/<br>

<br>

### 使用方法

1. 下载 heroku CLI 客户端: https://devcenter.heroku.com/articles/getting-started-with-php#set-up <br>
2. 部署 <br>
```
$ heroku login
$ git clone https://github.com/justsweetpotato/you2php-heroku.git 
# 修改 web/config.php 文件.
$ cd you2php-heroku 
$ heroku create [You APP Name]
$ heroku git:remote -a [You APP Name]
$ git add .<br>
$ git commit -am "make it better"
$ git push heroku master
$ heroku ps:scale web=1
$ heroku open
 ```
<br>

