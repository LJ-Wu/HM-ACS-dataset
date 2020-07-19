Chinese version
这里以30order_2depot_data.xls为例解释每个sheet的含义。

1.sheet location依次包含了2个冷库和30个订单目的地的地理位置。 

2.sheet distance和sheet duration则分别依次包含了32个地点两两之间的驾驶距离和时间，同一地点之间的驾驶距离和时间设置为0，单位分别为米和秒。如sheet distance的第一行数据代表的是第一个冷库到其他所有地点的驾驶距离，第三行数据则代表第一个订单目的地到其他所有地点的驾驶距离，以此类推。

3.sheet A1，A2和A3则分别代表3个不同的测试样例，其中每个订单可根据其索引从sheet location中获取相应的订单目的地地理位置，同样地，也可根据冷库索引获取相应的冷库地理位置。如sheet A1中索引为1的订单对应的目的地地理位置为sheet location的第三行数据，（116.332117，39.950482），其对应的冷库索引为1，即第二个冷库，可以得知其地理位置为sheet location的第二行数据，（116.356622，39.949487）。

-----------------------------------------------------------------------------------------------------------------------------------------------------
English version
Taking 30order_2depot_data.xls as an example 

1. The geographical location information of 2 depots and 30 order destinations are included in the sheet 'location', where the first two locations represent the depot.

2. The driving distance and duration among 32 locations are included in sheet 'distance' and sheet 'duration' respectively. The distance and duration between the same location are 0. Besides, the basic unit of distance is meter while it is second for duration. Note that data of (row(i), column(j)) in sheet 'distance' represents the driving distance from location i to location j. Similar for sheet 'duration'.

3. sheet 'A1', 'A2', and 'A3' represent three different instances that share the same geographical location and driving information. That is, each order of 'A1', 'A2', and 'A3' can get the order destination as well as the depot location from the sheet 'location' according to its index. Then, driving information can be obtained from sheet 'distance' and sheet 'duration'. For example, the destination location of the order with index 1 in sheet 'A1' is (116.332117, 39.950482), which is the data of the 3rd row in sheet 'location'. Since the corresponding depot index is 1, that is, the second depot, we can know that its location is (116.356622, 39.949487), the data of the 2nd row in sheet 'location'.
