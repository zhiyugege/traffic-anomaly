# 交通异常检测相关文章和数据集
|  ID  | 数据集 |       方法       |                          补充                          | 时序 |
| :--: | :----: | :--------------: | :----------------------------------------------------: | :--: |
| P.1  |  D.1   | 有监督、分割任务 |          基于贝叶斯的方法来表述物体的运动模式          |  无  |
| P.2  |  D.2   | 有监督、检测任务 |           行车过程中突然闯入的行人的异常检测           |  无  |
| P.3  |  D.3   |   有监督、分析   |    异常检测流水线；分析行车速度、方向、间距作为特征    |  有  |
| P.4  |  D.4   |   半监督、分类   |             基于车辆运行轨迹的异常检测+svm             |  有  |
| P.5  |  D.5   |   半监督、分类   |                基于光流的直方图特征+svm                |  有  |
| P.6  |  D.6   |   有监督、分析   |     基于模糊交通参数（车流、密度、运动模式）和规则     |  有  |
| p.7  |  D.7   |   半监督、分类   |                基于光流的直方图特征+svm                |  有  |
| P.8  |  D.8   |   无监督、分析   |           目标检测获取物体后if then分析异常            |  有  |
| P.9  |  D.8   |   无监督、分析   | 提出两个模块分别用于检测静态（停靠）和动态（变道）异常 |  有  |


|  ID  |                            文章名                            | 链接 |
| :--: | :----------------------------------------------------------: | ---- |
| P.1  | Anomaly Detection in Traffic Scenes via Spatial-Aware Motion Reconstruction | 2017 |
| P.2  | Detection of Sudden Pedestrian Crossings for Driving Assistance Systems | 2012 |
| P.3  | Computer Vison Based Road Trafﬁc Accident and Anomaly Detection in the Context of Bangladesh | 2014 |
| P.4  | Anomaly Detection on Traffic Videos Based on Trajectory Simplification | 2013 |
| P.5  |    Optical Flow Based Anomaly Detection in Traffic Scenes    | 2017 |
| P.6  |     Road Traffic Anomaly Detection based on Fuzzy Theory     | 2018 |
| P.7  | Fast Anomaly Detection in Traffic Surveillance Video Based on Robust Sparse Optical Flow | 2016 |
| P.8  | Unsupervised Anomaly Detection for Trafﬁc Surveillance Based on Background Modeling | 2018 |
| P.9  | A Novel Methodology of Time Dependent Mean Field Based Multilayer Unsupervised Anomaly Detection Using Traffic Surveillance Videos | 2019 |


|  ID  | 类型 |                 异常类别                 |  标注   |    视角    |                             链接                             |
| :--: | :--: | :--------------------------------------: | :-----: | :--------: | :----------------------------------------------------------: |
| D.1  | 视频 | 车辆超车；车辆穿越；行人、摩托车穿越道路 |  像素   | 行车记录仪 |           [link](https://pan.baidu.com/s/1dG3Nxj7)           |
| D.2  | 视频 |            突然的行人穿越道路            |   帧    | 行车记录仪 |                              -                               |
| D.3  | 视频 |                   车祸                   |   帧    | 路口摄像头 |                              -                               |
| D.4  | 视频 |                无具体描述                |  视频   | 路口摄像头 |                              -                               |
| D.5  | 视频 |     车辆超车；车辆穿越；行人穿越道路     |   帧    | 行车记录仪 |                             ITS                              |
| D.6  | 视频 |     车辆逆行；行人穿越道路；行车拥挤     |  事件   | 路口摄像头 |                        SNA2014-Nomal                         |
| D.7  | 视频 |          车辆逆行；行人穿越道路          | 帧 像素 | 路口摄像头 | [UCSD ped1](http://pan.baidu.com/s/1pKFvlMz) |
| D.8  | 视频 |              车祸；车辆抛锚              |   帧    | 路口摄像头 | [NVIDIA aicity](http://www.aicitychallenge.org/track3-download/) |

Tips：

- 用直方图来描述物体的运动模式作为特征；

- sudden change

- 光流

- 基于svm的分类器

- 锚定，交通拥堵，交通事故和非法驾驶

- traffic parameters：traffic flow, traffic density, vehicle trajectory, speed, etc.

- 通过区分正常和异常运动模式来提高异常检测类别的多样性

-  1、大多数异常检测算法只能在某一个数据集上work；2、其次，交通监控中对异常检测的需求要能够胜任各种场景，而这是任何现有方法都无法实现的。

- UA-DETRAC 车辆目标检测数据集

- 对于固定的摄像头视角，例如路口摄像头，可以用基于光流的方法提取背景和运动的目标

- 在文章p9中提出了三大类异常和对应的算法特点：事故（关注车辆的异常移动：方向或速度变化）；非法停靠（速度变化）；超速（速度变化）和非法变道（车辆的异常移动：方向）
