# 企业网站/APP后台<a name="sfs_01_0054"></a>

## 场景介绍<a name="section5877142785112"></a>

对于I/O密集型的网站业务，SFS Turbo为多个Web Server提供共享的网站源码目录，存储，提供低延迟，高IOPS的并发共享访问能力。业务特点：

-   大量小文件：存放网站静态文件，包括HTML文件，Json文件，静态图片等。
-   读I/O密集：业务以小文件读为主，数据写入相对较少。
-   多个Web Server访问同一个SFS Turbo后台，实现网站业务的高可用。

## 配置流程<a name="section203761746155216"></a>

1.  整理好网站文件。
2.  登录弹性文件服务控制台，创建一个SFS Turbo文件系统用于存放网站文件。
3.  登录作为计算节点的云服务器，挂载文件系统。
4.  通过头节点将需要上传的网站文件上传到挂载的文件系统。
5.  启动Web Server。

## 前提条件<a name="section17422148155316"></a>

-   已完成VPC创建。
-   已完成作为头节点和计算节点的云服务器创建并将其归属在已创建的VPC下。
-   已开通SFS Turbo服务。

## 配置参考<a name="section1036721911570"></a>

1.  登录弹性文件服务管理控制台。
2.  在页面右上角单击“创建文件系统“。
3.  在创建文件系统页面，根据界面提示配置参数。
4.  配置完成后，单击“立即创建”，完成文件系统创建。

    Linux系统ECS挂载操作请参见[挂载NFS文件系统到云服务器（Linux）](https://support.huaweicloud.com/qs-sfs/zh-cn_topic_0034428728.html)；Windows系统ECS挂载操作请参见[挂载NFS文件系统到云服务器（Windows）](https://support.huaweicloud.com/qs-sfs/zh-cn_topic_0105224109.html)和[挂载CIFS文件系统到云服务器（Windows）](https://support.huaweicloud.com/qs-sfs/zh-cn_topic_0151246279.html)。

5.  登录头节点将需要上传的网站文件上传到挂载的文件系统。
6.  启动Web Server。

