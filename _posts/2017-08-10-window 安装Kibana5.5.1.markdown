#安装Kibana 5.5.1（Windows）

* 安装Kibana 5.5.1:
下载：
https://www.elastic.co/cn/downloads/kibana
kibana-5.5.1-windows-x86.zip
*  解压；F:\java\elasticsearch\kibana-5.5.1-windows-x86
*  修改配置：F:\java\elasticsearch\kibana-5.5.1-windows-x86\config\kibana.yml
设置elasticsearch.url为启动的elasticsearch实例
```
# The URL of the Elasticsearch instance to use for all your queries.
# elasticsearch.url: "http://localhost:9200"
elasticsearch.url: "http://localhost:9200"
```
*  启动：F:\java\elasticsearch\kibana-5.5.1-windows-x86\bin\kibana.bat **必须先启动elasticsearch**
到kibana-5.5.1-windows-x86\bin目录，双击kibana.bat
或者
cmd
cd kibana-5.5.1-windows-x86\bin
.\kibana.bat
![](http://orkwbnlu7.bkt.clouddn.com/QQ%E5%9B%BE%E7%89%8720170810155245.png)
*  访问：
http://localhost:5601
![](http://orkwbnlu7.bkt.clouddn.com/QQ%E5%9B%BE%E7%89%8720170810155422.png)

