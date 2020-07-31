# 配置多VPC<a name="sfs_01_0036"></a>

VPC为弹性云服务器构建隔离的、用户自主配置和管理的虚拟网络环境，提升用户云中资源的安全性，简化用户的网络部署。使用弹性文件服务时，文件系统和云服务器归属于同一VPC下才能文件共享。

VPC可以通过网络ACL进行访问控制。网络ACL是对一个或多个子网的访问控制策略系统，根据与子网关联的入站/出站规则，判断数据包是否被允许流入/流出关联子网。在文件系统的VPC列表中每添加一个授权地址并设置相应权限即创建了一个网络ACL。

现支持为SFS文件系统配置多个VPC，以使归属于不同VPC的云服务器，只要所属的VPC被添加到文件系统的VPC列表下，或云服务器被添加到了VPC的授权地址中，则实际上归属于不同VPC的云服务器也能共享访问同一个文件系统。

更多关于VPC的信息请参见[虚拟私有云 VPC](https://support.huaweicloud.com/vpc/index.html)。

## 使用限制<a name="section1888617013249"></a>

-   一个文件系统最多可以添加20个可用的VPC，对于添加的VPC所创建的ACL规则总和不能超过400个。添加VPC时会自动添加默认IP地址0.0.0.0/0。
-   如果已经在VPC控制台删除文件系统绑定的VPC，该VPC在文件系统绑定的VPC列表下可见且授权的IP地址/地址段为“激活”状态，但此时该VPC已无法进行使用，建议将该VPC从列表中删除。
-   SFS Turbo文件系统暂不支持配置多VPC。

## 操作步骤<a name="section696112185365"></a>

1.  登录弹性文件服务管理控制台。
2.  在文件系统列表中单击目标文件系统名称，进入授权VPC界面。
3.  如果没有可用的VPC，需要先申请VPC。可以为文件系统添加多个VPC，单击“添加VPC“，弹出“添加VPC“对话框。如[图1](#fig625115289418)所示。

    可以在下拉列表中选中多个VPC。

    **图 1**  添加VPC<a name="fig625115289418"></a>  
    ![](figures/添加VPC.png "添加VPC")

4.  单击“确定“，完成添加。添加成功的VPC会出现在列表中，添加VPC时会自动添加默认IP地址0.0.0.0/0，默认读写权限为“读写”，默认用户权限为“no\_all\_squash”，默认用户root权限为“no\_root\_squash”。
5.  在VPC列表下可以看到所有添加的VPC的信息，参数说明如[表1](#table99851739124510)所示。

    **表 1**  参数说明

    <a name="table99851739124510"></a>
    <table><thead align="left"><tr id="row18986439164514"><th class="cellrowborder" valign="top" width="27.889999999999997%" id="mcps1.2.3.1.1"><p id="p13986133914512"><a name="p13986133914512"></a><a name="p13986133914512"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="72.11%" id="mcps1.2.3.1.2"><p id="p2986193915452"><a name="p2986193915452"></a><a name="p2986193915452"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row159865391455"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.3.1.1 "><p id="p4986163914454"><a name="p4986163914454"></a><a name="p4986163914454"></a>名称</p>
    </td>
    <td class="cellrowborder" valign="top" width="72.11%" headers="mcps1.2.3.1.2 "><p id="p398663944512"><a name="p398663944512"></a><a name="p398663944512"></a>已添加的VPC的名称，例如：vpc-4040。</p>
    </td>
    </tr>
    <tr id="row1398615399451"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.3.1.1 "><p id="p1998693919458"><a name="p1998693919458"></a><a name="p1998693919458"></a>授权IP数量</p>
    </td>
    <td class="cellrowborder" valign="top" width="72.11%" headers="mcps1.2.3.1.2 "><p id="p2986939164516"><a name="p2986939164516"></a><a name="p2986939164516"></a>已经添加的IP地址或IP地址段的个数。</p>
    </td>
    </tr>
    <tr id="row498693904514"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.3.1.1 "><p id="p1998643964514"><a name="p1998643964514"></a><a name="p1998643964514"></a>操作</p>
    </td>
    <td class="cellrowborder" valign="top" width="72.11%" headers="mcps1.2.3.1.2 "><p id="p55891167164624"><a name="p55891167164624"></a><a name="p55891167164624"></a>包含“添加”和“删除”操作。“添加”即添加授权的IP地址，包括对授权的IP地址、读/写权限、用户权限、用户root权限及优先级的设置，请参见<a href="#table1242824684814">表2</a>。“删除”即删除该VPC。</p>
    </td>
    </tr>
    </tbody>
    </table>

6.  单击VPC名称左边的![](figures/icon-down.png)，可以查看目标VPC添加的IP地址/地址段的详细信息。可以对其进行添加、编辑和删除IP地址/地址段的操作。在目标VPC的“操作“列，单击“添加“，弹出“添加授权地址”的弹窗，如[图2](#fig87801322188)所示。可以根据参数说明如[表2](#table1242824684814)所示完成添加。

    **图 2**  添加授权地址<a name="fig87801322188"></a>  
    ![](figures/添加授权地址.png "添加授权地址")

    **表 2**  参数说明

    <a name="table1242824684814"></a>
    <table><thead align="left"><tr id="row18428154644810"><th class="cellrowborder" valign="top" width="25%" id="mcps1.2.3.1.1"><p id="p842884615488"><a name="p842884615488"></a><a name="p842884615488"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="75%" id="mcps1.2.3.1.2"><p id="p19428104612489"><a name="p19428104612489"></a><a name="p19428104612489"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row242814617489"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.3.1.1 "><p id="p11428104616485"><a name="p11428104616485"></a><a name="p11428104616485"></a>授权地址</p>
    </td>
    <td class="cellrowborder" valign="top" width="75%" headers="mcps1.2.3.1.2 "><a name="ul13324116192216"></a><a name="ul13324116192216"></a><ul id="ul13324116192216"><li>只能输入一个IPv4地址/地址段。</li><li>输入的IPv4地址/地址段必须合法，且不能为除0.0.0.0/0以外之前0开头的IP地址或地址段，其中当设置为0.0.0.0/0时表示VPC内的任意IP。同时，不能为127以及224~255开头的IP地址或地址段，例如127.0.0.1，224.0.0.1，255.255.255.255，因为以224-239开头的IP地址或地址段是属于D类地址，用于组播；以240-255开头的IP地址或地址段属于E类地址，用于研究。使用非合法的IP或IP地址段可能会导致添加访问规则失败或者添加的访问规则无法生效。</li><li>无法输入多个地址，如：10.0.1.32,10.5.5.10用逗号分隔等形式的多个地址。</li><li>如果要表示一个地址段，如192.168.1.0-192.168.1.255的地址段应使用掩码形式：192.168.1.0/24，不支持192.168.1.0-255等其他地址段表示形式。掩码位数的取值为0到31的整数，且只有为0.0.0.0/0时掩码位数可取0，其他情况均不合法。</li></ul>
    </td>
    </tr>
    <tr id="row144285465480"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.3.1.1 "><p id="p4428946144813"><a name="p4428946144813"></a><a name="p4428946144813"></a>读或写权限</p>
    </td>
    <td class="cellrowborder" valign="top" width="75%" headers="mcps1.2.3.1.2 "><p id="p144281746204810"><a name="p144281746204810"></a><a name="p144281746204810"></a>分为读写权限和只读权限。默认为“读写”。</p>
    </td>
    </tr>
    <tr id="row4428104634818"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.3.1.1 "><p id="p242894610484"><a name="p242894610484"></a><a name="p242894610484"></a>用户权限</p>
    </td>
    <td class="cellrowborder" valign="top" width="75%" headers="mcps1.2.3.1.2 "><p id="p144285462480"><a name="p144285462480"></a><a name="p144285462480"></a>设置是否保留共享目录的UID和GID。默认为“no_all_squash”。</p>
    <a name="ul1829105884712"></a><a name="ul1829105884712"></a><ul id="ul1829105884712"><li>all_squash：共享文件的UID（User ID）和GID（Group ID）映射给nobody用户，适合公共目录。</li><li>no_all_squash：保留共享文件的UID和GID。</li></ul>
    <p id="p169142811244"><a name="p169142811244"></a><a name="p169142811244"></a>CIFS类型的文件系统添加授权地址时，不涉及该参数。</p>
    </td>
    </tr>
    <tr id="row1942884614813"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.3.1.1 "><p id="p442816468484"><a name="p442816468484"></a><a name="p442816468484"></a>用户root权限</p>
    </td>
    <td class="cellrowborder" valign="top" width="75%" headers="mcps1.2.3.1.2 "><p id="p19428446204818"><a name="p19428446204818"></a><a name="p19428446204818"></a>设置是否允许客户端的root权限。默认为“no_root_squash”。</p>
    <a name="ul202950116498"></a><a name="ul202950116498"></a><ul id="ul202950116498"><li>root_squash：不允许客户端以root用户访问，客户端使用root用户访问时映射为nobody用户。</li><li>no_root_squash：允许客户端以root用户访问，root用户具有根目录的完全控制访问权限。</li></ul>
    <p id="p99331427192715"><a name="p99331427192715"></a><a name="p99331427192715"></a>CIFS类型的文件系统添加授权地址时，不涉及该参数。</p>
    </td>
    </tr>
    <tr id="row144282465483"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.3.1.1 "><p id="p1542834624815"><a name="p1542834624815"></a><a name="p1542834624815"></a>优先级</p>
    </td>
    <td class="cellrowborder" valign="top" width="75%" headers="mcps1.2.3.1.2 "><p id="p20428114604814"><a name="p20428114604814"></a><a name="p20428114604814"></a>优先级只能是0-100的整数。0表示优先级最高，100表示优先级最低。同一VPC内挂载时会优先使用该优先级高的IP地址/地址段所拥有的权限，存在相同优先级时会优先匹配最新添加或修改的IP地址/地址段。例如：用户在执行挂载操作时的IP地址为10.1.1.32，而在已经授权的IP地址/地址段中10.1.1.32（读写）优先级为100和10.1.1.0/24（只读）优先级为50均符合要求，则用户权限会使用优先级为50的10.1.1.0/24（只读）的只读权限。10.1.1.0/24内的所有地址包括10.1.1.32，在无其他授权优先级的情况下，则将会使用优先级为50的10.1.1.0/24（只读）的只读权限。</p>
    </td>
    </tr>
    </tbody>
    </table>

    >![](public_sys-resources/icon-note.gif) **说明：**   
    >属于VPC A中的弹性云服务器IP地址可以被成功添加至VPC B的授权IP地址内，但该云服务器无法挂载属于VPC B下的文件系统。弹性云服务器和文件系统所使用的VPC需为同一个。  


