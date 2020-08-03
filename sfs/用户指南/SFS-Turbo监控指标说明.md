# SFS Turbo监控指标说明<a name="sfs_01_0048"></a>

## 功能说明<a name="section59820001153251"></a>

本节定义了云文件上报云监控的监控指标的命名空间，监控指标列表和维度定义，用户可以通过管理控制台或云监控提供的[API接口](https://support.huaweicloud.com/api-ces/zh-cn_topic_0171212514.html)来查询监控指标。

## 命名空间<a name="section172651386227"></a>

SYS.EFS

## 监控指标<a name="section18266133811225"></a>

<a name="table102675383222"></a>
<table><thead align="left"><tr id="row726893842214"><th class="cellrowborder" valign="top" width="15.151515151515152%" id="mcps1.1.6.1.1"><p id="p20269183892219"><a name="p20269183892219"></a><a name="p20269183892219"></a>指标</p>
</th>
<th class="cellrowborder" valign="top" width="16.161616161616163%" id="mcps1.1.6.1.2"><p id="p16270153816220"><a name="p16270153816220"></a><a name="p16270153816220"></a>指标名称</p>
</th>
<th class="cellrowborder" valign="top" width="36.36363636363637%" id="mcps1.1.6.1.3"><p id="p527115383221"><a name="p527115383221"></a><a name="p527115383221"></a>含义</p>
</th>
<th class="cellrowborder" valign="top" width="11.111111111111112%" id="mcps1.1.6.1.4"><p id="p202711238192210"><a name="p202711238192210"></a><a name="p202711238192210"></a>取值范围</p>
</th>
<th class="cellrowborder" valign="top" width="21.21212121212121%" id="mcps1.1.6.1.5"><p id="p52723385226"><a name="p52723385226"></a><a name="p52723385226"></a>测量对象</p>
</th>
</tr>
</thead>
<tbody><tr id="row2272193812219"><td class="cellrowborder" valign="top" width="15.151515151515152%" headers="mcps1.1.6.1.1 "><p id="p1267882881318"><a name="p1267882881318"></a><a name="p1267882881318"></a>client_connections</p>
</td>
<td class="cellrowborder" valign="top" width="16.161616161616163%" headers="mcps1.1.6.1.2 "><p id="p1967816281134"><a name="p1967816281134"></a><a name="p1967816281134"></a>客户端连接数</p>
</td>
<td class="cellrowborder" valign="top" width="36.36363636363637%" headers="mcps1.1.6.1.3 "><p id="p17678202861320"><a name="p17678202861320"></a><a name="p17678202861320"></a>该指标用于统计测量客户端连接数。</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.1.6.1.4 "><p id="p133881228195216"><a name="p133881228195216"></a><a name="p133881228195216"></a>≥ 0</p>
</td>
<td class="cellrowborder" valign="top" width="21.21212121212121%" headers="mcps1.1.6.1.5 "><p id="p1567872871317"><a name="p1567872871317"></a><a name="p1567872871317"></a>云文件</p>
</td>
</tr>
<tr id="row22801038122214"><td class="cellrowborder" valign="top" width="15.151515151515152%" headers="mcps1.1.6.1.1 "><p id="p5678128131318"><a name="p5678128131318"></a><a name="p5678128131318"></a>data_read_io_bytes</p>
</td>
<td class="cellrowborder" valign="top" width="16.161616161616163%" headers="mcps1.1.6.1.2 "><p id="p1467882861312"><a name="p1467882861312"></a><a name="p1467882861312"></a>读带宽</p>
</td>
<td class="cellrowborder" valign="top" width="36.36363636363637%" headers="mcps1.1.6.1.3 "><p id="p16678228181317"><a name="p16678228181317"></a><a name="p16678228181317"></a>该指标用于测量读I/O负载。</p>
<p id="p5696614174714"><a name="p5696614174714"></a><a name="p5696614174714"></a>单位：byte/s</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.1.6.1.4 "><p id="p8678112818136"><a name="p8678112818136"></a><a name="p8678112818136"></a>≥ 0 bytes/s</p>
</td>
<td class="cellrowborder" valign="top" width="21.21212121212121%" headers="mcps1.1.6.1.5 "><p id="p17678122817134"><a name="p17678122817134"></a><a name="p17678122817134"></a>云文件</p>
</td>
</tr>
<tr id="row16283638112211"><td class="cellrowborder" valign="top" width="15.151515151515152%" headers="mcps1.1.6.1.1 "><p id="p26781128151310"><a name="p26781128151310"></a><a name="p26781128151310"></a>data_write_io_bytes</p>
</td>
<td class="cellrowborder" valign="top" width="16.161616161616163%" headers="mcps1.1.6.1.2 "><p id="p10143416258"><a name="p10143416258"></a><a name="p10143416258"></a>写带宽</p>
</td>
<td class="cellrowborder" valign="top" width="36.36363636363637%" headers="mcps1.1.6.1.3 "><p id="p6678328141317"><a name="p6678328141317"></a><a name="p6678328141317"></a>该指标用于测量写I/O负载。</p>
<p id="p12578141214478"><a name="p12578141214478"></a><a name="p12578141214478"></a>单位：byte/s</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.1.6.1.4 "><p id="p118291591311"><a name="p118291591311"></a><a name="p118291591311"></a>≥ 0 bytes/s</p>
</td>
<td class="cellrowborder" valign="top" width="21.21212121212121%" headers="mcps1.1.6.1.5 "><p id="p76781028151315"><a name="p76781028151315"></a><a name="p76781028151315"></a>云文件</p>
</td>
</tr>
<tr id="row102875381228"><td class="cellrowborder" valign="top" width="15.151515151515152%" headers="mcps1.1.6.1.1 "><p id="p1867922841312"><a name="p1867922841312"></a><a name="p1867922841312"></a>metadata_io_bytes</p>
</td>
<td class="cellrowborder" valign="top" width="16.161616161616163%" headers="mcps1.1.6.1.2 "><p id="p11679328131314"><a name="p11679328131314"></a><a name="p11679328131314"></a>元数据读写带宽</p>
</td>
<td class="cellrowborder" valign="top" width="36.36363636363637%" headers="mcps1.1.6.1.3 "><p id="p18679528131312"><a name="p18679528131312"></a><a name="p18679528131312"></a>该指标用于测量元数据读写I/O负载。</p>
<p id="p85163108475"><a name="p85163108475"></a><a name="p85163108475"></a>单位：byte/s</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.1.6.1.4 "><p id="p196791728171317"><a name="p196791728171317"></a><a name="p196791728171317"></a>≥ 0 bytes/s</p>
</td>
<td class="cellrowborder" valign="top" width="21.21212121212121%" headers="mcps1.1.6.1.5 "><p id="p667932811136"><a name="p667932811136"></a><a name="p667932811136"></a>云文件</p>
</td>
</tr>
<tr id="row1037910119139"><td class="cellrowborder" valign="top" width="15.151515151515152%" headers="mcps1.1.6.1.1 "><p id="p967982818139"><a name="p967982818139"></a><a name="p967982818139"></a>total_io_bytes</p>
</td>
<td class="cellrowborder" valign="top" width="16.161616161616163%" headers="mcps1.1.6.1.2 "><p id="p136791128101315"><a name="p136791128101315"></a><a name="p136791128101315"></a>总带宽</p>
</td>
<td class="cellrowborder" valign="top" width="36.36363636363637%" headers="mcps1.1.6.1.3 "><p id="p196796286134"><a name="p196796286134"></a><a name="p196796286134"></a>该指标用于测量总I/O负载。</p>
<p id="p1634916814714"><a name="p1634916814714"></a><a name="p1634916814714"></a>单位：byte/s</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.1.6.1.4 "><p id="p2067914289131"><a name="p2067914289131"></a><a name="p2067914289131"></a>≥ 0 bytes/s</p>
</td>
<td class="cellrowborder" valign="top" width="21.21212121212121%" headers="mcps1.1.6.1.5 "><p id="p26796283138"><a name="p26796283138"></a><a name="p26796283138"></a>云文件</p>
</td>
</tr>
<tr id="row31591714161313"><td class="cellrowborder" valign="top" width="15.151515151515152%" headers="mcps1.1.6.1.1 "><p id="p267932801318"><a name="p267932801318"></a><a name="p267932801318"></a>iops</p>
</td>
<td class="cellrowborder" valign="top" width="16.161616161616163%" headers="mcps1.1.6.1.2 "><p id="p155709312265"><a name="p155709312265"></a><a name="p155709312265"></a>IOPS</p>
</td>
<td class="cellrowborder" valign="top" width="36.36363636363637%" headers="mcps1.1.6.1.3 "><p id="p767914289139"><a name="p767914289139"></a><a name="p767914289139"></a>该指标用于测量单位时间内处理的I/O数。</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.1.6.1.4 "><p id="p76791128151310"><a name="p76791128151310"></a><a name="p76791128151310"></a>≥ 0</p>
</td>
<td class="cellrowborder" valign="top" width="21.21212121212121%" headers="mcps1.1.6.1.5 "><p id="p11679162881316"><a name="p11679162881316"></a><a name="p11679162881316"></a>云文件</p>
</td>
</tr>
<tr id="row13829184911438"><td class="cellrowborder" valign="top" width="15.151515151515152%" headers="mcps1.1.6.1.1 "><p id="p19829134914319"><a name="p19829134914319"></a><a name="p19829134914319"></a>used_capacity</p>
</td>
<td class="cellrowborder" valign="top" width="16.161616161616163%" headers="mcps1.1.6.1.2 "><p id="p1829849204310"><a name="p1829849204310"></a><a name="p1829849204310"></a>已用容量</p>
</td>
<td class="cellrowborder" valign="top" width="36.36363636363637%" headers="mcps1.1.6.1.3 "><p id="p582917498435"><a name="p582917498435"></a><a name="p582917498435"></a>该指标用于统计文件系统已用容量。</p>
<p id="p813713324610"><a name="p813713324610"></a><a name="p813713324610"></a>单位：byte</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.1.6.1.4 "><p id="p10829104919436"><a name="p10829104919436"></a><a name="p10829104919436"></a>≥ 0 bytes</p>
</td>
<td class="cellrowborder" valign="top" width="21.21212121212121%" headers="mcps1.1.6.1.5 "><p id="p3504163484812"><a name="p3504163484812"></a><a name="p3504163484812"></a>云文件</p>
</td>
</tr>
<tr id="row5677125244310"><td class="cellrowborder" valign="top" width="15.151515151515152%" headers="mcps1.1.6.1.1 "><p id="p1367745214311"><a name="p1367745214311"></a><a name="p1367745214311"></a>used_capacity_percent</p>
</td>
<td class="cellrowborder" valign="top" width="16.161616161616163%" headers="mcps1.1.6.1.2 "><p id="p66771652194319"><a name="p66771652194319"></a><a name="p66771652194319"></a>容量使用率</p>
</td>
<td class="cellrowborder" valign="top" width="36.36363636363637%" headers="mcps1.1.6.1.3 "><p id="p16677195214439"><a name="p16677195214439"></a><a name="p16677195214439"></a>该指标用于统计文件系统已用容量占总容量的比例。</p>
<p id="p2836185518459"><a name="p2836185518459"></a><a name="p2836185518459"></a>单位：百分比</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.1.6.1.4 "><p id="p1767785214316"><a name="p1767785214316"></a><a name="p1767785214316"></a>0 - 100%</p>
</td>
<td class="cellrowborder" valign="top" width="21.21212121212121%" headers="mcps1.1.6.1.5 "><p id="p16504103417488"><a name="p16504103417488"></a><a name="p16504103417488"></a>云文件</p>
</td>
</tr>
</tbody>
</table>

## 维度<a name="section102905383226"></a>

<a name="table13291038182217"></a>
<table><thead align="left"><tr id="row13292153862219"><th class="cellrowborder" valign="top" width="40.400000000000006%" id="mcps1.1.3.1.1"><p id="p17292638192211"><a name="p17292638192211"></a><a name="p17292638192211"></a>Key</p>
</th>
<th class="cellrowborder" valign="top" width="59.599999999999994%" id="mcps1.1.3.1.2"><p id="p92938385226"><a name="p92938385226"></a><a name="p92938385226"></a>Value</p>
</th>
</tr>
</thead>
<tbody><tr id="row1429373812228"><td class="cellrowborder" valign="top" width="40.400000000000006%" headers="mcps1.1.3.1.1 "><p id="p1493610247242"><a name="p1493610247242"></a><a name="p1493610247242"></a>efs_instance_id</p>
</td>
<td class="cellrowborder" valign="top" width="59.599999999999994%" headers="mcps1.1.3.1.2 "><p id="p13649721326"><a name="p13649721326"></a><a name="p13649721326"></a>实例</p>
</td>
</tr>
</tbody>
</table>

## 查看监控数据<a name="section6170132094711"></a>

1.  登录管理控制台。
2.  进入监控图表页面。
    -   入口一：选择“存储 \> 弹性文件服务”，在文件系统列表单击查看监控数据的文件系统“操作”列下的“查看监控指标”。
    -   入口二：选择“管理与部署 \> 云监控服务\> 云服务监控 \> 云文件”，在文件系统列表中，单击待查看监控数据的文件系统“操作”列下的“查看监控指标”。

3.  您可以选择监控指标项或者监控时间段，查看对应的SFS Turbo监控数据。

    SFS Turbo监控图标如[图1](#fig18339242154716)所示，关于云监控的其他操作和更多信息，请参考《云监控用户指南》。

    **图 1**  SFS Turbo监控图表<a name="fig18339242154716"></a>  
    ![](figures/SFS-Turbo监控图表.png "SFS-Turbo监控图表")


