# 交通异常检测相关文章和数据集
|    ID    |  数据集   |       方法       |                             补充                             | 时序 |
| :------: | :-------: | :--------------: | :----------------------------------------------------------: | :--: |
|   P.1    |    D.1    | 有监督、分割任务 |             基于贝叶斯的方法来表述物体的运动模式             |  无  |
|   P.2    |    D.2    | 有监督、检测任务 |              行车过程中突然闯入的行人的异常检测              |  无  |
|   P.3    |    D.3    |   有监督、分析   |       异常检测流水线；分析行车速度、方向、间距作为特征       |  有  |
|   P.4    |    D.4    |   半监督、分类   |                基于车辆运行轨迹的异常检测+svm                |  有  |
|   P.5    |    D.5    |   半监督、分类   |                   基于光流的直方图特征+svm                   |  有  |
|   P.6    |    D.6    |   有监督、分析   |        基于模糊交通参数（车流、密度、运动模式）和规则        |  有  |
|   p.7    |    D.7    |   半监督、分类   |                   基于光流的直方图特征+svm                   |  有  |
|   P.8    |    D.8    |   无监督、分析   |              目标检测获取物体后if then分析异常               |  有  |
|   P.9    |    D.8    |   无监督、分析   |    提出两个模块分别用于检测静态（停靠）和动态（变道）异常    |  有  |
|   P.10   |    D.7    |   无监督、分析   | decode-encode+restruction error(对于无异常情况的时间序列 autoencoder) |  有  |
|   P.11   |   D.11    |   无监督、分析   |     decode-encode+restruction error（时间相关稀疏编码）      |  有  |
|   P.12   |    D.7    |   有监督、分析   |   利用时间、空间的mixture dynamic textures 提出UCSD ped1 2   |  有  |
|   P.13   | D.7、D.10 |   有监督、分析   |                 基于光流的直方图特征+最近邻                  |  有  |
|   P.14   | D.7、D.10 |   无监督、分析   | decode-encode+restruction error（fully convolutional autoencoder.） |  有  |
| **P.15** | D.7、D.9  |   有监督、分类   |              预训练得到概念感知、分类、异常描述              |  无  |
|   P.16   | D.7、D.10 |   无监督、分析   |                    sparse respresentation                    |  有  |
|   P.17   |   D.11    |   有监督、分析   |            video prediction by GAN(空间+光流信息)            |  有  |
|   P.18   |   D.12    |   无监督、分析   |                trajectories tracking 非法左转                |  有  |
|   P.19   |     -     |   无监督、分析   |         intelligent driver model+particle advection          |  有  |
|   P.20   |     -     |   有监督、分析   |           利用相邻车辆的交通变量进行异常检测和分类           |  有  |
|   P.21   |   D.13    |   有监督、检测   |                 交通事故预测的新数据集和loss                 |  有  |


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
| P.10 | Abnormal Event Detection in Videos Using Spatiotemporal Autoencoder | 2017 |
| P.11 | A Revisit of Sparse Coding Based Anomaly Detection in Stacked RNN Framework | 2017 |
| P.12 |             Anomaly Detection in Crowded Scenes              | 2010 |
| P.13 | Histograms of Optical Flow Orientation and Magnitude and Entropy to Detect Anomalous Events in Videos | 2016 |
| P.14 |       Learning Temporal Regularity in Video Sequences        | 2016 |
| P.15 | Joint Detection and Recounting of Abnormal Events by Learning Deep Generic Knowledge | 2017 |
| P.16 |   Sparse Reconstruction Cost for Abnormal Event Detection    | 2011 |
| P.17 | Future Frame Prediction for Anomaly Detection – A New Baseline | 2018 |
| P.18 | Crossroad Trafﬁc Surveillance Using Superpixel Tracking and Vehicle Trajectory Analysis | 2014 |
| P.19 |  Abnormal Traffic Detection using Intelligent Driver Model   | 2010 |
| P.20 | Distributed Classiﬁcation of Trafﬁc Anomalies Using Microscopic Trafﬁc Variables | 2013 |
| P.21 | Anticipating Trafﬁc Accidents with Adaptive Loss and Large-scale Incident DB | 2018 |


|  ID  | type |                 异常类别                 |    标注    |    视角    |                             链接                             |
| :--: | :--: | :--------------------------------------: | :--------: | :--------: | :----------------------------------------------------------: |
| D.1  | 视频 | 车辆超车；车辆穿越；行人、摩托车穿越道路 |    像素    | 行车记录仪 |           [link](https://pan.baidu.com/s/1dG3Nxj7)           |
| D.2  | 视频 |            突然的行人穿越道路            |     帧     | 行车记录仪 |                              -                               |
| D.3  | 视频 |                   车祸                   |     帧     | 路口摄像头 |                              -                               |
| D.4  | 视频 |                无具体描述                |    视频    | 路口摄像头 |                              -                               |
| D.5  | 视频 |     车辆超车；车辆穿越；行人穿越道路     |     帧     | 行车记录仪 |                             ITS                              |
| D.6  | 视频 |     车辆逆行；行人穿越道路；行车拥挤     |    事件    | 路口摄像头 |                        SNA2014-Nomal                         |
| D.7  | 视频 |          车辆逆行；行人穿越道路          |  帧 像素   | 路口摄像头 |        [UCSD ped1 2](http://pan.baidu.com/s/1pKFvlMz)        |
| D.8  | 视频 |              车祸；车辆抛锚              |     帧     | 路口摄像头 | [NVIDIA aicity](http://www.aicitychallenge.org/track3-download/) |
| D.9  | 视频 |    行人游荡、乱跑、扔杂物（行人only）    |     帧     | 路口摄像头 |                         CUHK Avenue                          |
| D.10 | 视频 |      行人走错方向、游荡（行人only）      |     帧     | 路口摄像头 |                            Subway                            |
| D.11 | 视频 |               D.7+D.9+D.10               |  帧 像素   | 路口摄像头 | [shanghaitech](https://onedrive.live.com/?authkey=%21AMqh2fTSemfrokE&id=3705E349C336415F%215109&cid=3705E349C336415F) |
| D.12 | 视频 |                 非法转向                 |   边界框   | 路口摄像头 |                           PETS2001                           |
| D.13 | 视频 |         行人、自行车、机动车相撞         | 帧、边界框 | 行车记录仪 |                             NIDB                             |



