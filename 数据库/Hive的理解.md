# 对于Hive的理解

## 基于HDFS的数据仓库工具
	可以将数据文件映射为数据库表
	将HiveQL转化为MapReduce任务

## 对于其他数据源的集成
	数据源需要在HDFS结构中, 可以将数据源文件根据Dirver解析成数据库表
	例如: mongodb, mysql, Hbase

## Hbase
	基于zk集群的数据库存储格式
	put逐个字段存储, 按行写入; 即当存在缺失字段时, 写入失败
	利用phoenixdb可以封装Hbase之后进行sql查询
