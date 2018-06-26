这是数据处理的部分。
数据文件介绍：
	1.	港湾大道.xlsx ：包括18个路口点的中心坐标、交叉路口各个方向的路径坐标，以及各个方向的路名。比如银坑是个十字路口，有四个方向点ABCD，分别对应 港湾大道南	港湾大道北	泉星东路	银泉山庄路 这四个名称
	2.	18个路口人流量数据汇总.xlsx ： 包括四个sheet,分别是每个路口的每个方向周末、周末24小时、工作日、工作日24小时的人流量统计数据。
	3.	gangwang_dadao_read_excel.py ： 对数据进行处理的python源文件
	4.	lukou_data_gangwan.json ： 最终生成的JSON数据文件

处理目的：
	将数据处理成JSON文件，提供前端使用。数据的大概结构：
		1.	主干：18个路口点的坐标、以及各个方向组成的人流量线路
		2.	分支：各个路口的各个方向分支周末和工作日的人流量统计数据