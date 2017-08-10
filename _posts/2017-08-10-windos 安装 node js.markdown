### 1、安装node环境
> 网址：https://nodejs.org/en/download/ 下载Windows版msi的
![图片](http://orkwbnlu7.bkt.clouddn.com/QQ%E5%9B%BE%E7%89%8720170810141318.png)

![图片](http://orkwbnlu7.bkt.clouddn.com/QQ%E5%9B%BE%E7%89%8720170810141724.png)

### 2.配置node的环境变量
> 需要配置2个地方 上图中的
``F:\java\nodejs 的node.exe`` 和 ``F:\java\nodejs\node_modules\npm\bin 的npm.cmd ``
![图片](http://orkwbnlu7.bkt.clouddn.com/QQ%E5%9B%BE%E7%89%8720170810142129.png)

``NODE_PATH:F:\java\nodejs;F:\java\nodejs\node_modules\npm\bin``

![图片](http://orkwbnlu7.bkt.clouddn.com/QQ%E5%9B%BE%E7%89%8720170810142235.png)

``path:%NODE_PATH%;``

配置成功后，运行 node -v 、npm -v 、appium -v 都成功了

![](http://orkwbnlu7.bkt.clouddn.com/QQ%E5%9B%BE%E7%89%8720170810142456.png)

### 3.npm太慢， 使用淘宝npm镜像使用方法
***淘宝 npm 地址： http://npm.taobao.org/***
>1.临时使用
``npm --registry https://registry.npm.taobao.org install express``
>2.持久使用
``npm config set registry https://registry.npm.taobao.org``
```
F:\java\nodejs>npm config set registry https://registry.npm.taobao.org

配置后可通过下面方式来验证是否成功 
npm config get registry
或 
npm info express
F:\java\nodejs>npm config get registry
https://registry.npm.taobao.org/
```
>3.通过cnpm使用
``npm install -g cnpm --registry=https://registry.npm.taobao.org``
使用 
``cnpm install express``
####测试：
```
F:\java\nodejs>npm install -g grunt-cli
C:\Users\wanghaibo\AppData\Roaming\npm\grunt -> C:\Users\wanghaibo\AppData\Roaming\npm\node_modules\grunt-cli\bin\grunt
C:\Users\wanghaibo\AppData\Roaming\npm
`-- grunt-cli@1.2.0
  +-- findup-sync@0.3.0
  | `-- glob@5.0.15
  |   +-- inflight@1.0.6
  |   | `-- wrappy@1.0.2
  |   +-- inherits@2.0.3
  |   +-- minimatch@3.0.4
  |   | `-- brace-expansion@1.1.8
  |   |   +-- balanced-match@1.0.0
  |   |   `-- concat-map@0.0.1
  |   +-- once@1.4.0
  |   `-- path-is-absolute@1.0.1
  +-- grunt-known-options@1.1.0
  +-- nopt@3.0.6
  | `-- abbrev@1.1.0
  `-- resolve@1.1.7
```