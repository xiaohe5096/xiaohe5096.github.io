#安装ElasticSearch 5.5.1（Windows）

* 安装ElasticSearch 5.5.1:
下载：从官网下载ElasticSearch https://www.elastic.co/downloads/elasticsearch，下载zip。
elasticsearch-5.5.1.zip
*  解压到``F:\java\elasticsearch\elasticsearch-5.5.1``
文件夹的解释：
| Type   | 	Description	| Default Location| 	Setting| 
| -------|--------------|-----------------|------------|
| home   | 	elasticsearch主目录(`$ES_HOME`)|	解压软件包自动创建| 	
| bin    | 	elasticsearch启动节点启动脚本,elasticsearch-plugin插件安装脚本|		`$ES_HOME/bin`| 	
| conf   | 	配置文件，包含elasticsearch.yml|		`$ES_HOME/config`	|	path.conf| 
| data   | 	节点上分配的每个index/shard的数据文件的位置,可以有多个位置|		`$ES_HOME/data`	|	path.data| 
| logs   | 	日志文件的存放位置|		`$ES_HOME/logs`|		path.logs| 
| plugins| 	插件文件的位置，每个插件一个子文件夹|		`$ES_HOME/plugins`	| 
| repo   | 	共享文件系统存储库位置,容纳多个位置。可以放置在此处指定的任何目录的任何子目录中。|	Not  configured	|	path.repo| 
| script|		脚本文件的位置|		`$ES_HOME/scripts`|		path.scripts| 

*  进入到``F:\java\elasticsearch\elasticsearch-5.5.1\bin执行elasticsearch.bat``
*  本机就启动了一个ElasticSearch节点，启动后会显示如图所示
![](http://orkwbnlu7.bkt.clouddn.com/QQ%E5%9B%BE%E7%89%8720170810160208.png)
* 打开浏览器里测试一下
![](http://orkwbnlu7.bkt.clouddn.com/QQ%E5%9B%BE%E7%89%8720170810160541.png)
