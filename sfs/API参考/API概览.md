# API概览<a name="sfs_02_0007"></a>

弹性文件服务所提供的接口分为SFS接口、SFS Turbo接口与OpenStack原生接口。

通过配合使用弹性文件服务所提供的接口和OpenStack原生接口，您可以完整的使用弹性文件服务的所有功能。

SFS接口调用频率限制为：400次/分钟。若您需要调用的接口较多，可能存在因限频出现拉取失败的情况，建议尽量将请求按时间维度均摊。

本服务接口，与mitaka版本的openstack组件manila部分接口相同，相关接口使用方式也可以参考开源社区接口说明，链接地址：

[https://docs.openstack.org/api-ref/shared-file-system/](https://docs.openstack.org/api-ref/shared-file-system/)。

使用企业项目功能时，关于SFS API 接口是否支持企业项目，请参考[API授权项列表](SFS授权项分类.md)。

**当本文描述内容与上述开源社区的描述不一致时，请以本文描述为准。**

**表 1**  接口说明

<a name="table5876102613294"></a>
<table><thead align="left"><tr id="row3878122616298"><th class="cellrowborder" valign="top" width="12.6%" id="mcps1.2.5.1.1"><p id="p443403145110"><a name="p443403145110"></a><a name="p443403145110"></a>文进系统类型</p>
</th>
<th class="cellrowborder" valign="top" width="15.97%" id="mcps1.2.5.1.2"><p id="p487811268290"><a name="p487811268290"></a><a name="p487811268290"></a><strong id="b1251874443714"><a name="b1251874443714"></a><a name="b1251874443714"></a>接口类型</strong></p>
</th>
<th class="cellrowborder" valign="top" width="16.49%" id="mcps1.2.5.1.3"><p id="p68781126182914"><a name="p68781126182914"></a><a name="p68781126182914"></a><strong id="b125201844173712"><a name="b125201844173712"></a><a name="b125201844173712"></a>子类型</strong></p>
</th>
<th class="cellrowborder" valign="top" width="54.94%" id="mcps1.2.5.1.4"><p id="p158781726112914"><a name="p158781726112914"></a><a name="p158781726112914"></a><strong id="b15203449370"><a name="b15203449370"></a><a name="b15203449370"></a>说明</strong></p>
</th>
</tr>
</thead>
<tbody><tr id="row148781026122919"><td class="cellrowborder" valign="top" width="12.6%" headers="mcps1.2.5.1.1 "><p id="p15434113119518"><a name="p15434113119518"></a><a name="p15434113119518"></a>SFS</p>
</td>
<td class="cellrowborder" valign="top" width="15.97%" headers="mcps1.2.5.1.2 "><p id="p16878726162916"><a name="p16878726162916"></a><a name="p16878726162916"></a>SFS接口</p>
</td>
<td class="cellrowborder" valign="top" width="16.49%" headers="mcps1.2.5.1.3 "><p id="p128788265295"><a name="p128788265295"></a><a name="p128788265295"></a>共享标签</p>
</td>
<td class="cellrowborder" valign="top" width="54.94%" headers="mcps1.2.5.1.4 "><p id="p1810154210242"><a name="p1810154210242"></a><a name="p1810154210242"></a>共享标签可供给用户对共享进行自定义标记。通过共享标签，用户可以自由地对共享分类管理。</p>
</td>
</tr>
<tr id="row9878726192911"><td class="cellrowborder" rowspan="5" valign="top" width="12.6%" headers="mcps1.2.5.1.1 "><p id="p8731165814531"><a name="p8731165814531"></a><a name="p8731165814531"></a>SFS</p>
</td>
<td class="cellrowborder" rowspan="5" valign="top" width="15.97%" headers="mcps1.2.5.1.2 "><p id="p1587832642913"><a name="p1587832642913"></a><a name="p1587832642913"></a>OpenStack原生接口</p>
</td>
<td class="cellrowborder" valign="top" width="16.49%" headers="mcps1.2.5.1.3 "><p id="p17341921193318"><a name="p17341921193318"></a><a name="p17341921193318"></a>查询API版本</p>
</td>
<td class="cellrowborder" valign="top" width="54.94%" headers="mcps1.2.5.1.4 "><p id="p14101184217244"><a name="p14101184217244"></a><a name="p14101184217244"></a>通过这些接口，可以查询所有API的版本和API版本的详细信息。</p>
</td>
</tr>
<tr id="row9878172662914"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="p1310194211243"><a name="p1310194211243"></a><a name="p1310194211243"></a>文件共享</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="p58589475242"><a name="p58589475242"></a><a name="p58589475242"></a>通过这些接口，您可以创建共享，可获取共享的详细信息，如共享挂载路径等。</p>
</td>
</tr>
<tr id="row117351143103220"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="p15101134272411"><a name="p15101134272411"></a><a name="p15101134272411"></a>共享访问规则</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="p610144252418"><a name="p610144252418"></a><a name="p610144252418"></a>通过这些接口，您可以添加和修改、删除共享的访问规则，如配置VPC等。</p>
</td>
</tr>
<tr id="row11736144363213"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="p51011542102411"><a name="p51011542102411"></a><a name="p51011542102411"></a>配额管理</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="p20101542202416"><a name="p20101542202416"></a><a name="p20101542202416"></a>如果创建共享的个数已经到达上限，您可以通过这些接口，对相关配额进行修改。</p>
</td>
</tr>
<tr id="row1685181354019"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="p768516135406"><a name="p768516135406"></a><a name="p768516135406"></a>扩容缩容</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="p136851513144016"><a name="p136851513144016"></a><a name="p136851513144016"></a>若需要改变已创建的共享的容量大小，您可以通过这些接口，实现文件共享的扩容和缩容。</p>
</td>
</tr>
<tr id="row1391016615534"><td class="cellrowborder" rowspan="2" valign="top" width="12.6%" headers="mcps1.2.5.1.1 "><p id="p191117625319"><a name="p191117625319"></a><a name="p191117625319"></a>SFS Turbo</p>
</td>
<td class="cellrowborder" rowspan="2" valign="top" width="15.97%" headers="mcps1.2.5.1.2 "><p id="p1391115685315"><a name="p1391115685315"></a><a name="p1391115685315"></a>SFS Turbo接口</p>
</td>
<td class="cellrowborder" valign="top" width="16.49%" headers="mcps1.2.5.1.3 "><p id="p0234152816542"><a name="p0234152816542"></a><a name="p0234152816542"></a>生命周期管理</p>
</td>
<td class="cellrowborder" valign="top" width="54.94%" headers="mcps1.2.5.1.4 "><p id="p11911164535"><a name="p11911164535"></a><a name="p11911164535"></a>包括创建文件系统、删除文件系统、查询文件系统列表、查询文件系统详情等接口。</p>
</td>
</tr>
<tr id="row1094814242531"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="p294922465316"><a name="p294922465316"></a><a name="p294922465316"></a>存储容量管理</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="p10522129105513"><a name="p10522129105513"></a><a name="p10522129105513"></a>对指定的文件系统进行扩容操作。</p>
</td>
</tr>
</tbody>
</table>

