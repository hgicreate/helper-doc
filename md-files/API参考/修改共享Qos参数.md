# 修改共享Qos参数<a name="sfs_02_0048"></a>

## 功能介绍<a name="section10684447163819"></a>

修改指定共享的Qos参数。

## URI<a name="section1665327514513"></a>

-   PUT /v2/\{project\_id\}/shares/\{share\_id\}/metadata
-   参数说明

    <a name="table22021759152019"></a>
    <table><thead align="left"><tr id="row16139965152019"><th class="cellrowborder" valign="top" width="18.56%" id="mcps1.1.5.1.1"><p id="p17124101410431"><a name="p17124101410431"></a><a name="p17124101410431"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="13.4%" id="mcps1.1.5.1.2"><p id="p1612415146430"><a name="p1612415146430"></a><a name="p1612415146430"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.65%" id="mcps1.1.5.1.3"><p id="p312416148432"><a name="p312416148432"></a><a name="p312416148432"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="46.39%" id="mcps1.1.5.1.4"><p id="p3124181464318"><a name="p3124181464318"></a><a name="p3124181464318"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row55089343152019"><td class="cellrowborder" valign="top" width="18.56%" headers="mcps1.1.5.1.1 "><p id="p1781134044818"><a name="p1781134044818"></a><a name="p1781134044818"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="13.4%" headers="mcps1.1.5.1.2 "><p id="p59952126152019"><a name="p59952126152019"></a><a name="p59952126152019"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.65%" headers="mcps1.1.5.1.3 "><p id="p24284048152019"><a name="p24284048152019"></a><a name="p24284048152019"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.39%" headers="mcps1.1.5.1.4 "><p id="p20850895152019"><a name="p20850895152019"></a><a name="p20850895152019"></a>操作用户的项目ID，获取方法请参见<a href="获取项目ID.md">获取项目ID</a>。</p>
    </td>
    </tr>
    <tr id="row3119103219486"><td class="cellrowborder" valign="top" width="18.56%" headers="mcps1.1.5.1.1 "><p id="p1011933217487"><a name="p1011933217487"></a><a name="p1011933217487"></a>share_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="13.4%" headers="mcps1.1.5.1.2 "><p id="p18120163210481"><a name="p18120163210481"></a><a name="p18120163210481"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.65%" headers="mcps1.1.5.1.3 "><p id="p11120113294813"><a name="p11120113294813"></a><a name="p11120113294813"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.39%" headers="mcps1.1.5.1.4 "><p id="p13120143211489"><a name="p13120143211489"></a><a name="p13120143211489"></a>共享ID。</p>
    </td>
    </tr>
    </tbody>
    </table>


## 请求消息<a name="section5063604914513"></a>

-   参数说明

    <a name="table1836815510524"></a>
    <table><thead align="left"><tr id="row1137265565217"><th class="cellrowborder" valign="top" width="16.33%" id="mcps1.1.5.1.1"><p id="p9445335122519"><a name="p9445335122519"></a><a name="p9445335122519"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="19.39%" id="mcps1.1.5.1.2"><p id="p194456353258"><a name="p194456353258"></a><a name="p194456353258"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="12.24%" id="mcps1.1.5.1.3"><p id="p12445335152517"><a name="p12445335152517"></a><a name="p12445335152517"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="52.04%" id="mcps1.1.5.1.4"><p id="p1344583582512"><a name="p1344583582512"></a><a name="p1344583582512"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row8379125520523"><td class="cellrowborder" valign="top" width="16.33%" headers="mcps1.1.5.1.1 "><p id="p13380755115210"><a name="p13380755115210"></a><a name="p13380755115210"></a>metadata</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.1.5.1.2 "><p id="p1038255513523"><a name="p1038255513523"></a><a name="p1038255513523"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="12.24%" headers="mcps1.1.5.1.3 "><p id="p18383165518521"><a name="p18383165518521"></a><a name="p18383165518521"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="52.04%" headers="mcps1.1.5.1.4 "><p id="p938455505218"><a name="p938455505218"></a><a name="p938455505218"></a>设置共享的起始容量参数。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   metadata字段说明：

    <a name="t02fa2a8d319442e18936e45a4b0868e9"></a>
    <table><thead align="left"><tr id="r0d59edb1d3b84778ac0d399ba307cea3"><th class="cellrowborder" valign="top" width="16.220000000000002%" id="mcps1.1.5.1.1"><p id="p89501128115014"><a name="p89501128115014"></a><a name="p89501128115014"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="12.78%" id="mcps1.1.5.1.2"><p id="p15950132815504"><a name="p15950132815504"></a><a name="p15950132815504"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="20%" id="mcps1.1.5.1.3"><p id="p12966112865014"><a name="p12966112865014"></a><a name="p12966112865014"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="51%" id="mcps1.1.5.1.4"><p id="p4966172895016"><a name="p4966172895016"></a><a name="p4966172895016"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="r51c142ecbaf2461ba473dee4939fca92"><td class="cellrowborder" valign="top" width="16.220000000000002%" headers="mcps1.1.5.1.1 "><p id="p830161474317"><a name="p830161474317"></a><a name="p830161474317"></a>#sfs_min_capacity</p>
    </td>
    <td class="cellrowborder" valign="top" width="12.78%" headers="mcps1.1.5.1.2 "><p id="acedc2a0b65b64463b4ceecbe0a4c8fff"><a name="acedc2a0b65b64463b4ceecbe0a4c8fff"></a><a name="acedc2a0b65b64463b4ceecbe0a4c8fff"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.5.1.3 "><p id="ae54b1ae095b34db0a389cf59563b381e"><a name="ae54b1ae095b34db0a389cf59563b381e"></a><a name="ae54b1ae095b34db0a389cf59563b381e"></a><span>Integer</span></p>
    </td>
    <td class="cellrowborder" valign="top" width="51%" headers="mcps1.1.5.1.4 "><p id="p206765417432"><a name="p206765417432"></a><a name="p206765417432"></a>起始容量，用户预设置的共享最小使用容量，基于该容量进行Qos控制，该值越大，文件读写带宽越大。取值范围[40, 512000]，单位GB。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   请求样例

    ```
    {
      "metadata" : {
        "#sfs_min_capacity" : 50
      }
    }
    ```


## 响应消息<a name="section6408307814513"></a>

-   参数说明

    <a name="table65331262558"></a>
    <table><thead align="left"><tr id="row4533162625518"><th class="cellrowborder" valign="top" width="16.33%" id="mcps1.1.5.1.1"><p id="p653342665511"><a name="p653342665511"></a><a name="p653342665511"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="19.39%" id="mcps1.1.5.1.2"><p id="p165331226105519"><a name="p165331226105519"></a><a name="p165331226105519"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="12.24%" id="mcps1.1.5.1.3"><p id="p5533826145520"><a name="p5533826145520"></a><a name="p5533826145520"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="52.04%" id="mcps1.1.5.1.4"><p id="p453318261551"><a name="p453318261551"></a><a name="p453318261551"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row053342615554"><td class="cellrowborder" valign="top" width="16.33%" headers="mcps1.1.5.1.1 "><p id="p65332026175517"><a name="p65332026175517"></a><a name="p65332026175517"></a>metadata</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.1.5.1.2 "><p id="p953311261556"><a name="p953311261556"></a><a name="p953311261556"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="12.24%" headers="mcps1.1.5.1.3 "><p id="p45334266554"><a name="p45334266554"></a><a name="p45334266554"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="52.04%" headers="mcps1.1.5.1.4 "><p id="p38511304393"><a name="p38511304393"></a><a name="p38511304393"></a>共享的起始容量参数。</p>
    </td>
    </tr>
    </tbody>
    </table>


-   响应样例

    ```
    {
      "metadata" : {
        "#sfs_min_capacity" : 50
      }
    }
    ```


## 状态码<a name="section4959408514513"></a>

-   正常

    204

-   异常

    <a name="table6245403714513"></a>
    <table><thead align="left"><tr id="row1507735814513"><th class="cellrowborder" valign="top" width="43.43%" id="mcps1.1.3.1.1"><p id="p1330652014513"><a name="p1330652014513"></a><a name="p1330652014513"></a>状态码</p>
    </th>
    <th class="cellrowborder" valign="top" width="56.57%" id="mcps1.1.3.1.2"><p id="p408636314513"><a name="p408636314513"></a><a name="p408636314513"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row3477393214513"><td class="cellrowborder" valign="top" width="43.43%" headers="mcps1.1.3.1.1 "><p id="p6522508214513"><a name="p6522508214513"></a><a name="p6522508214513"></a>400 Bad Request</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.57%" headers="mcps1.1.3.1.2 "><p id="p4874025614513"><a name="p4874025614513"></a><a name="p4874025614513"></a>无效输入。</p>
    </td>
    </tr>
    <tr id="row3600912414513"><td class="cellrowborder" valign="top" width="43.43%" headers="mcps1.1.3.1.1 "><p id="p3105792214513"><a name="p3105792214513"></a><a name="p3105792214513"></a>401 Unauthorized</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.57%" headers="mcps1.1.3.1.2 "><p id="p3266375714513"><a name="p3266375714513"></a><a name="p3266375714513"></a>鉴权失败。</p>
    </td>
    </tr>
    <tr id="row2553835814513"><td class="cellrowborder" valign="top" width="43.43%" headers="mcps1.1.3.1.1 "><p id="p5534113514513"><a name="p5534113514513"></a><a name="p5534113514513"></a>403 Forbidden</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.57%" headers="mcps1.1.3.1.2 "><p id="p5344692014513"><a name="p5344692014513"></a><a name="p5344692014513"></a>对被请求页面的访问被禁止。</p>
    </td>
    </tr>
    <tr id="row1126023214513"><td class="cellrowborder" valign="top" width="43.43%" headers="mcps1.1.3.1.1 "><p id="p3966357214513"><a name="p3966357214513"></a><a name="p3966357214513"></a>404 Not Found</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.57%" headers="mcps1.1.3.1.2 "><p id="p5863278914513"><a name="p5863278914513"></a><a name="p5863278914513"></a>资源未找到。</p>
    </td>
    </tr>
    <tr id="row1011562214513"><td class="cellrowborder" valign="top" width="43.43%" headers="mcps1.1.3.1.1 "><p id="p1405905414513"><a name="p1405905414513"></a><a name="p1405905414513"></a>500 Internal Server Error</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.57%" headers="mcps1.1.3.1.2 "><p id="p6504160314513"><a name="p6504160314513"></a><a name="p6504160314513"></a>请求未完成。服务异常。</p>
    </td>
    </tr>
    </tbody>
    </table>


