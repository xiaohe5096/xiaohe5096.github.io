###1、安装node环境
> 网址：https://nodejs.org/en/download/ 下载Windows版msi的
![图片](http://orkwbnlu7.bkt.clouddn.com/QQ%E5%9B%BE%E7%89%8720170810141318.png)

![图片](http://orkwbnlu7.bkt.clouddn.com/QQ%E5%9B%BE%E7%89%8720170810141724.png)

###2.配置node的环境变量
> 需要配置2个地方 上图中的
``F:\java\nodejs 的node.exe`` 和 ``F:\java\nodejs\node_modules\npm\bin 的npm.cmd ``
![图片](http://orkwbnlu7.bkt.clouddn.com/QQ%E5%9B%BE%E7%89%8720170810142129.png)

``NODE_PATH:F:\java\nodejs;F:\java\nodejs\node_modules\npm\bin``

![图片](http://orkwbnlu7.bkt.clouddn.com/QQ%E5%9B%BE%E7%89%8720170810142235.png)

``path:%NODE_PATH%;``

配置成功后，运行 node -v 、npm -v 、appium -v 都成功了

![](http://orkwbnlu7.bkt.clouddn.com/QQ%E5%9B%BE%E7%89%8720170810142456.png)