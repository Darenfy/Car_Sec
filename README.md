# Car_Sec
Something About Car Security Research

[前置知识](https://github.com/Darenfy/Car_Sec/blob/main/%E8%BD%A6%E8%81%94%E7%BD%91%E5%AE%89%E5%85%A8%E5%89%8D%E7%BD%AE%E7%9F%A5%E8%AF%86.html)

## 汽车基础知识  
#### [车辆识别号码 ``VIN``](https://baike.baidu.com/item/%E8%BD%A6%E8%BE%86%E8%AF%86%E5%88%AB%E5%8F%B7%E7%A0%81/4338309?fromtitle=%E6%B1%BD%E8%BD%A6VIN%E7%A0%81&fromid=10965781)  
``Vehicle Idenfication Number``，即车辆识别号码，或俗称车架号码，主要用来区分汽车，号码独一无二。
> 30 年内制造的任何两辆车都不可能具有相同的 VIN

``VIN`` 包括十七个字母或数字，能够识别汽车的生产商、引擎、底盘序号及其他性能等资料。  
> 注：为避免冲突
> 英文字母不使用 
> ``l``、``O``、``Q`` 
> 第十位生产型年不使用 ``l``，``O``，``Q``，``U``，``Z``，``0``

**识别号码结构**  
主要有两种制式，欧盟和北美  
![](https://bkimg.cdn.bcebos.com/pic/d31b0ef41bd5ad6e73ac79c981cb39dbb6fd3cbf?x-bce-process=image/watermark,image_d2F0ZXIvYmFpa2U3Mg==,g_7,xp_5,yp_5/format,f_auto)

首三位：  
``WMI(World Manufacturer Identifier)`` 主要用来识别生产商的名称及所在国家  

通用号码位：  
- 第九位为校验位  
- 第十位为车型年码  
- 第十一位为车辆组装工厂

根据不同国家或者汽车生产厂家，``VIN`` 会有细微不同

#### [车载网关 ``Tbox``](http://murata.eetrend.com/article/2019-09/1003013.html)  
``Telematics BOX``(T-BOX) 车载通信终端，汽车通过这个小盒子实现上网功能  

#### [车载综合信息系统 ``IVI``](https://zhuanlan.zhihu.com/p/149469194)  
``In-Vehicle Information``

**主流车载 OS**  
- WinCE 系统 -> 基本退出  
- QNX 系统 -> 市面上大部分采用 QNX  
- Linux 系统 -> Ford Sync, BMW X 系列  
- Android 系统  
- 华为 OS  
- 阿里 OS -> 上汽荣威系列  

**车载娱乐系统框架**  
硬件架构图  
![](https://pic1.zhimg.com/80/v2-d8d26ec303ff0cb0fafae2ca2ee2506c_1440w.jpg)

**主要功能模块**  
- 多媒体  
- 导航  
- ``connectivity`` 连接模块: 蓝牙/``WI-FI`` 连接功能  
- 映射功能：将手机屏幕直接映射到车机上面，实现双向控制  
- 人机交互  
- 车身信息显示与控制  
- ``ADAS`` 等辅助驾驶功能：全息影像、倒车影像、自动泊车等  
- 社交应用模块：第三方车载 ``APP`` 社内社交

#### [汽车数字钥匙](https://www.ifanr.com/1249189)  
一般采用 ``RFID`` 无线射频技术，在相关模块中均有无线通讯收发器，在一定距离内进行感应  

新型方式：手机虚拟钥匙主要包括三种，云钥匙、蓝牙钥匙、NFC 钥匙  

云钥匙：在手机和车辆均有网络连接的情况下，通过手机 APP 实现远程解闭锁、远程启动等操作。可以用来远程控车

蓝牙钥匙：通过蓝牙进行匹配，当手机 ``APP`` 开启或后台运行情况下靠近车辆，自动解锁车门。无网环境下启动

#### [车联网服务商/后台 ``TSP``](https://www.sohu.com/a/13141642_120865)  
``Telematics Service Provider`` 汽车远程服务提供商，主要提供车联网上层车机与下层内容提供商的安全连接服务  

#### [``CAN`` 总线](https://zhuanlan.zhihu.com/p/30657287)  
``Controller Area Network`` 控制器局域网络  

物理层传输介质一般使用双绞线，传输信号形式一般为差分信号

``CAN`` 总线中报文帧格式主要分两种：标准帧和拓展帧  
报文的发送类型常用为：周期型、事件型、混合型  

#### [汽车 ``OBD`` 接口](https://jingyan.baidu.com/article/09ea3ede649fc9c0aede39f9.html)  
``On-Board Diagnostic``

车载自动诊断系统，能够检测汽车运行过程中的发动机电控系统和车辆的其他功能模块的工作状况。利用该接口与电脑互联(需要通过类似“网关”的设备），能实时查看汽车数据、检测汽车故障。  
![](https://exp-picture.cdn.bcebos.com/92174dbbf82064fb19f129928e6104a354e96f4d.jpg?x-bce-process=image%2Fresize%2Cm_lfit%2Cw_500%2Climit_1%2Fquality%2Cq_80)  

#### [信通院车联网安全白皮书](http://www.caict.ac.cn/kxyj/qwfb/bps/201804/P020170921430215345026.pdf)  
车联网智能终端安全重点关注终端系统安全和 App 安全

## Anroid 应用分析  


## 蓝牙低功耗  


## MQTT  


## CV2X  

