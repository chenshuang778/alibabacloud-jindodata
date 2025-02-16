### 使用前须知
* 请参考 [Jindo DistCp 介绍](jindo_distcp_overview.md) 文章内容进行环境适配和工具包下载
* 假设您的 distcp 任务启动在源 HDFS 集群上，别的情况以此类推。首先检查两个 HDFS 集群的网络情况，保证两个集群的 namenode 和 datanode 的相关端口可以互通访问，您需要将目标 HDFS 集群的 dfs.datanode.address 和 fs.defaultFS 这两个参数对应的端口从源 HDFS 集群的防火墙移除，确保目标 HDFS 的上述端口在源 HDFS 集群上可以访问
* 检查域名情况，将目的 HDFS 集群的 hosts 信息配置在源 HDFS 的 hosts 文件中
* 如您在使用过程中遇到问题可参考 [Jindo DistCp 问题排查指南](jindo_distcp_QA_pre.md) 进行解决，也可 [新建 ISSUE](https://github.com/aliyun/alibabacloud-jindodata/issues/new) 向我们反馈

### 1、拷贝数据到 HDFS 上
您可以使用如下命令将 hdfs 上的目录拷贝到 OSS 上
```shell
hadoop jar jindo-distcp-3.7.2.jar --src /srchdfs/dir --dest hdfs://<ip/hostname>:port/dir/ --parallelism 10
```
* --src：源hdfs的路径
* --dest：目标hdfs的路径，支持 hdfs://<ip/hostname>:port/dir/ 形式
* --parallelism：任务并发大小，根据集群资源可调整

### 2、增量拷贝文件
如果 Distcp 任务因为各种原因中间失败了，而此时您想进行断点续传，只Copy剩下未Copy成功的文件。或者源端文件新增了部分文件，此时需要您在进行上一次 Distcp 任务完成后进行如下操作：
##### 使用 --update 命令
```shell
hadoop jar jindo-distcp-3.7.2.jar --src /srchdfs/dir --dest hdfs://<ip/hostname>:port/dir/ --update --parallelism 20
```
如果所有文件都传输完成，则会提示如下信息。
```
INFO distcp.JindoDistCp: Jindo DistCp job exit with 0.
```
### 3、YARN 队列及带宽选择
如您需要对 DistCp 作业使用的 YARN 队列和带宽进行限定，可用如下命令
```shell
hadoop jar jindo-distcp-3.7.2.jar --src /srchdfs/dir --dest hdfs://<ip/hostname>:port/dir/ --queue yarnQueue --bandwidth 100 --parallelism 10
```
* --queue：指定 YARN 队列的名称
* --bandwidth：指定单机限流带宽的大小，单位 MB

### 4、其他功能
如您需要其他使用其他功能，请参考
* [Jindo DistCp 进行数据迁移的使用说明](jindo_distcp_how_to.md)
* [Jindo DistCp 场景化使用指南](jindo_distcp_scenario_guidance.md)

