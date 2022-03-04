# JindoFSx 缓存系统用户文档

## 快速入门
* [JindoFSx 缓存系统快速入门](/docs/user/4.x/4.1.0/jindofsx/jindofsx_quickstart.md)
* [使用 JindoSDK C/C++ 访问 JindoFSx 缓存系统](/docs/user/4.x/4.2.0/jindofsx/csdk_quickstart.md) <span style="color:red">*[NEW]*</span>

## 集群部署
* [快速部署一个简单的 JindoFSx 缓存系统](/docs/user/4.x/4.1.0/jindofsx/deploy/deploy_jindofsx.md)
* [部署高可用 JindoFSx 缓存系统](/docs/user/4.x/4.1.0/jindofsx/deploy/deploy_jindofsx_ha.md)
* [基于 Prometheus + Grafana 搭建 JindoFSx 缓存系统可视化指标观测平台](/docs/user/4.x/4.1.0/jindofsx/jindofsx_metrics.md)

## 基本功能
#### 阿里云 OSS 缓存加速
* [阿里云 OSS 透明缓存加速](/docs/user/4.x/4.1.0/jindofsx/oss/jindofsx_on_oss.md)
* [阿里云 OSS 统一挂载缓存加速](/docs/user/4.x/4.1.0/jindofsx/oss/jindofsx_on_oss_fsx.md)

#### 阿里云 OSS-HDFS 服务（JindoFS 服务）缓存加速
* [阿里云 OSS-HDFS 服务（JindoFS 服务）透明缓存加速](/docs/user/4.x/4.1.0/jindofsx/jindofs/jindofsx_on_jindofs.md)
* [阿里云 OSS-HDFS 服务（JindoFS 服务）统一挂载缓存加速](/docs/user/4.x/4.1.0/jindofsx/jindofs/jindofsx_on_jindofs_fsx.md)

#### Apache HDFS 缓存加速 <span style="color:red">*[NEW]*</span>
* [Apache HDFS 透明缓存加速](/docs/user/4.x/4.2.0/jindofsx/hdfs/jindofsx_on_hdfs.md)
* [Apache HDFS 统一挂载缓存加速](/docs/user/4.x/4.2.0/jindofsx/hdfs/jindofsx_on_hdfs_fsx.md)

#### 阿里云文件存储 NAS 缓存加速 <span style="color:red">*[NEW]*</span>
* [阿里云文件存储 NAS 统一挂载缓存加速](/docs/user/4.x/4.2.0/jindofsx/nas/jindofsx_on_nas_fsx.md)

#### JindoFSx 客户端侧 P2P 加速
* [P2P 分布式下载缓存使用说明](/docs/user/4.x/4.1.0/jindofsx/jindofsx_p2p.md)
  
#### JindoShell CLI 支持
* [JindoShell CLI 支持 JindoFSx 使用说明](/docs/user/4.x/4.1.0/jindofsx/jindoshell_jindofsx_howto.md)

## 性能测试

## 大数据生态
#### Hadoop 组件
* [Hadoop 访问阿里云 OSS + JindoFSx 透明加速](/docs/user/4.x/4.1.0/jindofsx/hadoop/hadoop_with_oss.md)
* [Hadoop 访问阿里云 OSS-HDFS 服务（JindoFS 服务）+ JindoFSx 透明加速](/docs/user/4.x/4.1.0/jindofsx/hadoop/hadoop_with_dls.md)
* [Hadoop 访问 JindoFSx 统一挂载的数据](/docs/user/4.x/4.1.0/jindofsx/hadoop/hadoop_with_fsx.md)

#### Spark 组件
* [Spark 处理阿里云 OSS 上的数据 + JindoFSx 透明加速](/docs/user/4.x/4.1.0/jindofsx/spark/jindosdk_on_spark_oss.md)
* [Spark 处理阿里云 OSS-HDFS 服务（JindoFS 服务）上的数据 + JindoFSx 透明加速](/docs/user/4.x/4.1.0/jindofsx/spark/jindosdk_on_spark_dls.md)
* [Spark 处理 JindoFSx 统一挂载的数据](/docs/user/4.x/4.1.0/jindofsx/spark/jindosdk_on_spark_fsx.md)

#### Hive 组件
* [Hive 处理阿里云 OSS 上的数据 + JindoFSx 透明加速](/docs/user/4.x/4.1.0/jindofsx/hive/jindosdk_on_hive_oss.md)
* [Hive 处理阿里云 OSS-HDFS 服务（JindoFS 服务）上的数据 + JindoFSx 透明加速](/docs/user/4.x/4.1.0/jindofsx/hive/jindosdk_on_hive_dls.md)
* [Hive 处理 JindoFSx 统一挂载的数据](/docs/user/4.x/4.1.0/jindofsx/hive/jindosdk_on_hive_fsx.md)

#### Presto 组件
* [Presto 查询阿里云 OSS 上的数据 + JindoFSx 透明加速](/docs/user/4.x/4.1.0/jindofsx/presto/jindosdk_on_presto_oss.md)
* [Presto 查询阿里云 OSS-HDFS 服务（JindoFS 服务）上的数据 + JindoFSx 透明加速](/docs/user/4.x/4.1.0/jindofsx/presto/jindosdk_on_presto_dls.md)
* [Presto 查询 JindoFSx 统一挂载的数据](/docs/user/4.x/4.1.0/jindofsx/presto/jindosdk_on_presto_fsx.md)

#### Impala 组件
* [Impala 查询阿里云 OSS 上的数据 + JindoFSx 透明加速](/docs/user/4.x/4.1.0/jindofsx/impala/jindosdk_on_impala_oss.md)
* [Impala 查询阿里云 OSS-HDFS 服务（JindoFS 服务）上的数据 + JindoFSx 透明加速](/docs/user/4.x/4.1.0/jindofsx/impala/jindosdk_on_impala_dls.md)
* [Impala 查询 JindoFSx 统一挂载的数据](/docs/user/4.x/4.1.0/jindofsx/impala/jindosdk_on_impala_fsx.md)

#### HBase 组件
* [HBase 使用阿里云 OSS 作为底层存储 + JindoFSx 透明加速](/docs/user/4.x/4.1.0/jindofsx/hbase/jindosdk_on_hbase_oss.md)
* [HBase 使用阿里云 OSS-HDFS 服务（JindoFS 服务）作为底层存储 + JindoFSx 透明加速](/docs/user/4.x/4.1.0/jindofsx/hbase/jindosdk_on_hbase_dls.md)
* [HBase 使用 JindoFSx 统一挂载的数据](/docs/user/4.x/4.1.0/jindofsx/hbase/jindosdk_on_hbase_fsx.md)

## AI 生态
#### JindoFuse 使用
* [JindoFuse 读写 JindoFSx 缓存(oss://路径挂载)](/docs/user/4.x/4.1.0/jindofsx/jindo_fuse/jindo_fuse_on_oss.md)
* [JindoFuse 读写 JindoFSx 缓存(fsx://路径挂载)](/docs/user/4.x/4.1.0/jindofsx/jindo_fuse/jindo_fuse_on_fsx.md)

## 最佳实践
#### 使用 JindoTable 缓存 Hive 表或分区的数据 <span style="color:red">*[NEW]*</span>
* [使用 JindoTable 缓存 Hive 表或分区的数据](jindotable/table_cache.md)