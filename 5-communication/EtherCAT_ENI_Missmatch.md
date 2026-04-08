## 5.3. 板通信 (EtherCAT) 主控 ENI 不匹配

### 1. 概述

控制器通信配置与 ENI 文件不匹配。<br>
(ENI : EtherCAT 网络信息)

### 2. 成因

{% hint style="info" %}

控制器通信配置与配置的 ENI 文件不匹配。<br>

{% endhint %}

### 验证控制器通信配置。

控制器支持预定义的通信配置。如果通信连接配置不正确，则无法正常操作。<br>
此外，连接时区分 [IN] 和 [OUT] 通信连接器。
为了确保正确的通信，将“第一块板的 [OUT] 连接器”连接到“第二块板的 [IN] 连接器”。<br>

<strong>< 正确通信配置的示例 ></strong><br>

- 主控制模块(H6COM-T) ↔ **[IN]** 伺服安全板 (BD642)
- 主控制模块(H6COM-T) ↔ **[IN]** 伺服安全板 (BD642) **[OUT]** ↔ **[IN]** 用户 DIO 板(BD681)

<br>

<strong>< 不正确通信配置的示例 ></strong><br>

- 主控制模块(H6COM-T) ↔ **[OUT]** 伺服安全板(BD642)
- 主控制模块(H6COM-T) ↔ **[IN]** 伺服安全板(BD642) **[OUT]** ↔ **[OUT]** 用户 DIO 板(BD681)
- 主控制模块(H6COM-T) ↔ **[IN]** 用户 DIO 板(BD681) **[OUT]** ↔ **[IN]** 伺服安全板(BD642)

<br>

![](../_assets/5-Communication/BD642_EtherCAT_Connector.png)<br>
图 5.3.1 BD642 EtherCAT 连接器

<br>

![](../_assets/5-Communication/BD681_EtherCAT_Connector.png)<br>
图 5.3.2 BD681 EtherCAT 连接器

<br>

当通信连接配置正确时，控制器会在开机时自动选择 ENI 文件并尝试建立连接。<br>

如果 ENI 文件的内部设置不正确，可能建立通信但功能可能无法正常操作。
在此情况下，请更新控制器主控制模块(H6COM-T)的版本或联系我们的公司。<br>

要手动更改 ENI 文件选择，请在下面的 TP 菜单中配置。
更改设置后，重新启动控制器以使更改生效。

**- 菜单位置 : [system]-[5:Initialization]-[10:Controller Setting]**