简易测试
	本软件是基于LabVIEW开发的面向电子产品的测试软件，具有研发、工程、网页三种模式，多UUT多脚本编辑并结合终端、日志、变量、收藏夹、数据分析。致力于让中小企业可以快速提升开发测试效率，让测试变得简单容易。

LabVIEW Runtime Engine 2018	64bit
NI VISA	15.0.1


1 文件创建
通过菜单栏的《新建》或【新建文件】按钮，可弹出新建文件对话框

 ![image](https://user-images.githubusercontent.com/28834684/163667051-eb452fa3-f4d1-496b-bf86-03e6082cfef1.png)

可自定义文件名称、项目名称、项目阶段
文件可创建多个UUT，默认为UUT1
UUT结构如下：

 ![image](https://user-images.githubusercontent.com/28834684/163667058-d5e5ea7a-c1ae-40a2-9ced-fc44b7ff78ca.png)

2 属性配置
双击Property，可以添加库，选择【添加】库，将适用于所在文件的所有UUT，添加后，自动根据版本匹配左侧External Libraries中可以找到的库文件

 ![image](https://user-images.githubusercontent.com/28834684/163667064-2286bda5-875e-45ea-92df-119e170d0fe2.png)

属性页或UUT页，只要编辑，都有紫色的编辑图标出现，需要Ctrl+S保存后，图标消失

 ![image](https://user-images.githubusercontent.com/28834684/163667071-3a003c05-f0bf-4c2c-99c3-a2335c6fe213.png)

3 测试大项创建
新建文件后，显示于左侧项目树列表中，双击选中Main，激活打开UUT，右键Main，可以添加测试大项

 ![image](https://user-images.githubusercontent.com/28834684/163667074-b08e8fd1-43f5-423d-ae95-5e4d68768ef8.png)
![image](https://user-images.githubusercontent.com/28834684/163667076-c8577ed9-7d5a-4096-bda7-4c19d166b98b.png)

 
4 测试小项创建
测试小项，依赖于属性所选择的外部库

 ![image](https://user-images.githubusercontent.com/28834684/163667082-07d7613b-c693-4710-ad7b-08e60a7f7057.png)
![image](https://user-images.githubusercontent.com/28834684/163667083-fb478456-c22e-4ab3-b852-1b31057139f3.png)
选择所需添加的库函数后，会弹出配置参数对话框，支持执行，还原，参数配置，其中的数组变量取自所属UUT的Variables
5 测试小项编辑
双击或选择右侧【编辑】按钮，可编辑指定的测试小项

 ![image](https://user-images.githubusercontent.com/28834684/163667093-e8a34b2f-77c9-4bcf-a8e4-21c73ae0b1c4.png)

6 测试小项调试
选中小项，右键可运行、增加断点、忽略、失败循环、复制，粘贴、删除

 ![image](https://user-images.githubusercontent.com/28834684/163667106-e65d1e05-6dd6-4901-b42a-081d0e238904.png)

7 UUT调试

 ![image](https://user-images.githubusercontent.com/28834684/163667116-9ac139a2-8dab-45de-b678-47d5016f7e6b.png)

按照顺序，分别为“开始”“自检”“停止”“暂停”“单步”“失败暂停”“忽略错误”“单项调试”“json文本”“UUT调测配置”
8 创建变量
选择左侧每个UUT下的Variables，显示该UUT所对应的变量，可添加单字符串和字符串数组变量

 ![image](https://user-images.githubusercontent.com/28834684/163667120-6457ae1f-bcbd-4f58-8a02-c939aec8ad6b.png)

9 监测变量
点击左侧变量，可随时监测或修改该UUT的变量值

 ![image](https://user-images.githubusercontent.com/28834684/163667125-225d8ea3-d5d9-4ced-a4c7-400bbbb04c96.png)

10 测试日志
当数组变量选择下图已创建变量Demo后，点击执行，可通过左侧日志按钮，实时查看Array数组库，所对应的日志，意味着，任何一个库的任何一个方法，日志都是可以实时监测的，方便调试

 ![image](https://user-images.githubusercontent.com/28834684/163667130-bb42d689-984f-41cf-bd56-b47655fb60ef.png)

11 终端
终端功能，类似在线监测调试工具，可监测端口的生命全流程，任何一个库都可以增加自定义的终端（符合已制定规则即可）

 ![image](https://user-images.githubusercontent.com/28834684/163667136-752edce0-6c70-4685-a377-0f596d0edd38.png)

当新建串口终端时，既可以作为串口工具，又能够联通测试项，达到串口自打开到关闭，全程都在终端监测内

 ![image](https://user-images.githubusercontent.com/28834684/163667142-c622a1bf-a84e-44fa-a24b-4d3eaa5d5ed7.png)

12 收藏夹
UUT或者测试项都可以收藏到收藏夹中，随时导入或导出，方便组内同步

 ![image](https://user-images.githubusercontent.com/28834684/163667147-b9e09778-a4a6-42fa-a3a2-9957ca015d1c.png)


13 数据
当测试完成后，可以在数据页查看任何时候的历史数据与历史日志，且包含数值解析、散点图、CPK分析、耗时分析

 ![image](https://user-images.githubusercontent.com/28834684/163667156-82031953-c80e-419f-b3cc-4f8057742985.png)
![image](https://user-images.githubusercontent.com/28834684/163667160-251fd588-8173-4e65-9b98-7de2fe99e0fe.png)
![image](https://user-images.githubusercontent.com/28834684/163667165-c0ed2184-7034-4d18-9b9e-6bd730fd689e.png)

  
任何一个时间的任何一个测试项，都可以选择分析，结合散点数据与CPK，确定测试规格是否OK

 ![image](https://user-images.githubusercontent.com/28834684/163667170-64f44ade-9712-4e4c-bf98-e3daabe7633c.png)

耗时页可分析测试大项的耗时统计，找到最耗时的测试项

 ![image](https://user-images.githubusercontent.com/28834684/163667185-03485489-30b1-458d-92ff-dde8acd3c084.png)

