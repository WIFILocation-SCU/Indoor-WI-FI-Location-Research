##时间
2015.11.18##地点
二基楼B400教室##人物
邢津炜  徐品晶  马家固##实验环境
教室里分布了比较多的课桌课椅，每台课桌上有一台电脑。教室长16.1m，宽5.9m。以东北角为坐标轴原点，方向南为纵坐标，方向西为横坐标。路由器LinkA的坐标为(348.6,1404.8),LinkB的坐标为(24.4,1404.8)，LinkC的坐标为(696.8,567.6)。选取三个定位目标位置坐标分别为(241,1144.2)，(241,1032)，(348.6,696.8)。##实验器材
mac pro，TP-LINK路由器。##实验数据
见Data table##实验过程
滤波方面，采取了高斯滤波，实验发现高斯滤波之后保留下来的数据较少，在特殊情况下，不能代表样本分布情况，如sheet2.2以及3.3等。并且信号强度具有严重的左偏，高斯滤波不能对此做比较好的处理。
接下来按照对数传播模型，以11.15号采集得到的数据作为计算样本，得到传播模型参数为2.89。在此传播模型基础上，采用最小二乘法定位，定位精度有高有低。##定位结果
1. 目标位置（241,1144.2），定位结果(125.91,1298.09)，误差为1.92m   2. 目标位置 (241,1032)，定位结果(278.6,1130.46)，误差为1.05m   3. 目标位置（348.6,696.8），定位结果(395.84,421.5)，误差为2.75m   ##精度误差分析三组数据定位误差分别为1.92m，1.05m,2.75m。  
造成改误差的原因：
* 滤波方式不能处理信号左偏的特征，这种情况下处理得到的数据可能有所偏差。为了验证这种情况，可以对信号的左偏特征处理之后，再验证定位精度，或者人工将得到的数据增大一点，观察定位效果是否有所改进。
* 室内环境复杂，我们发现x轴方向的误差要小于y轴方向的误差，我们估计这是由于桌面电脑的分布，电脑平行于x轴分布，因此对x轴方向误差的影响要小于y轴方向的影响。                      