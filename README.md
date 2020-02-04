# 交通异常检测相关文章和数据集
|  ID  | 数据集 |       方法       |                             补充                             | 时序 |
| :--: | :----: | :--------------: | :----------------------------------------------------------: | :--: |
| P.1  |  D.1   | 有监督、分割任务 |             基于贝叶斯的方法来表述物体的运动模式             |  无  |
| P.2  |  D.2   | 有监督、检测任务 |              行车过程中突然闯入的行人的异常检测              |  无  |
| P.3  |  D.3   |   有监督、分析   |       异常检测流水线；分析行车速度、方向、间距作为特征       |  有  |
| P.4  |  D.4   |   半监督、分类   |                基于车辆运行轨迹的异常检测+svm                |  有  |
| P.5  |  D.5   |   半监督、分类   |                   基于光流的直方图特征+svm                   |  有  |
| P.6  |  D.6   |   有监督、分析   |        基于模糊交通参数（车流、密度、运动模式）和规则        |  有  |
| p.7  |  D.7   |   半监督、分类   |                   基于光流的直方图特征+svm                   |  有  |
| P.8  |  D.8   |   无监督、分析   |              目标检测获取物体后if then分析异常               |  有  |
| P.9  |  D.8   |   无监督、分析   |    提出两个模块分别用于检测静态（停靠）和动态（变道）异常    |  有  |
| P.10 |  D.7   |   无监督、分析   | decode-encode+restruction error(对于无异常情况的时间序列 autoencoder) |  有  |
| P.11 |  D.11  |   无监督、分析   |     decode-encode+restruction error（时间相关稀疏编码）      |  有  |
|      |        |                  |                                                              |      |
|      |        |                  |                                                              |      |
|      |        |                  |                                                              |      |
|      |        |                  |                                                              |      |
|      |        |                  |                                                              |      |
|      |        |                  |                                                              |      |
|      |        |                  |                                                              |      |
|      |        |                  |                                                              |      |

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
|      |                                                              |      |
|      |                                                              |      |
|      |                                                              |      |
|      |                                                              |      |
|      |                                                              |      |
|      |                                                              |      |
|      |                                                              |      |
|      |                                                              |      |

|  ID  | type |                 异常类别                 |  标注   |    视角    |                             链接                             |
| :--: | :--: | :--------------------------------------: | :-----: | :--------: | :----------------------------------------------------------: |
| D.1  | 视频 | 车辆超车；车辆穿越；行人、摩托车穿越道路 |  像素   | 行车记录仪 |           [link](https://pan.baidu.com/s/1dG3Nxj7)           |
| D.2  | 视频 |            突然的行人穿越道路            |   帧    | 行车记录仪 |                              -                               |
| D.3  | 视频 |                   车祸                   |   帧    | 路口摄像头 |                              -                               |
| D.4  | 视频 |                无具体描述                |  视频   | 路口摄像头 |                              -                               |
| D.5  | 视频 |     车辆超车；车辆穿越；行人穿越道路     |   帧    | 行车记录仪 |                             ITS                              |
| D.6  | 视频 |     车辆逆行；行人穿越道路；行车拥挤     |  事件   | 路口摄像头 |                        SNA2014-Nomal                         |
| D.7  | 视频 |          车辆逆行；行人穿越道路          | 帧 像素 | 路口摄像头 | [UCSD ped1 2](http://pan.baidu.com/s/1pKFvlMz) |
| D.8  | 视频 |              车祸；车辆抛锚              |   帧    | 路口摄像头 | [NVIDIA aicity](http://www.aicitychallenge.org/track3-download/) |
| D.9  | 视频 |    行人游荡、乱跑、扔杂物（行人only）    |   帧    | 路口摄像头 |                         CUHK Avenue                          |
| D.10 | 视频 |      行人走错方向、游荡（行人only）      |   帧    | 路口摄像头 |                            Subway                            |
| D.11 | 视频 |               D.7+D.9+D.10               | 帧 像素 | 路口摄像头 | [shanghaitech](https://onedrive.live.com/?authkey=%21AMqh2fTSemfrokE&id=3705E349C336415F%215109&cid=3705E349C336415F) |
|      |      |                                          |         |            |                                                              |
|      |      |                                          |         |            |                                                              |
|      |      |                                          |         |            |                                                              |
|      |      |                                          |         |            |                                                              |
|      |      |                                          |         |            |                                                              |
|      |      |                                          |         |            |                                                              |
|      |      |                                          |         |            |                                                              |
|      |      |                                          |         |            |                                                              |

Tips：

·用直方图来描述物体的运动模式作为特征；

·sudden change

·光流

·基于svm的分类器

·锚定，交通拥堵，交通事故和非法驾驶

·traffic parameters：traffic flow, traffic density, vehicle trajectory, speed, etc.

·通过区分正常和异常运动模式来提高异常检测类别的多样性

· 1、大多数异常检测算法只能在某一个数据集上work；2、其次，交通监控中对异常检测的需求要能够胜任各种场景，而这是任何现有方法都无法实现的。

·UA-DETRAC 车辆目标检测数据集

·对于固定的摄像头视角，例如路口摄像头，可以用基于光流的方法提取背景和运动的目标

·在文章p9中提出了三大类异常和对应的算法特点：事故（关注车辆的异常移动：方向或速度变化）；非法停靠（速度变化）；超速（速度变化）和非法变道（车辆的异常移动：方向）

·**applied to diﬀerent scenes.设计的方法需要**

·less organized trafﬁc environments 

·**评价指标** frame-level AUC ROC

·异常检测的方法：1.dictionary based(autoecoder) 

待调研的文章

·**Abnormal trafﬁc detection using intelligent driver model**

https://ieeexplore.ieee.org/document/5597797

·**Distributed classiﬁcation of trafﬁc anomalies using microscopic trafﬁc variables**

https://ieeexplore.ieee.org/document/6335477

·**Histograms of Oriented Optical Flow and Binet-Cauchy Kernels on Nonlinear Dynamical Systems for the Recognition of Human Actions**

https://ieeexplore.ieee.org/document/5206821

·**Early detection of the pedestrian’s intention to cross the street**

https://ieeexplore.ieee.org/document/6338797

·**Histograms of Optical Flow Orientation and Magnitude to Detect Anomalous Events in Videos ***

https://ieeexplore.ieee.org/document/7778165

·**Automatic Analysis of Vehicle Trajectory Applied to Visual Surveillance**

https://link.springer.com/chapter/10.1007/978-3-319-23814-2_11

·**Crossroad Traffic Surveillance Using Superpixel Tracking and Vehicle Trajectory Analysis**

https://ieeexplore.ieee.org/document/6977103

·**Vehicle Abnormal Behavior Detection System based on Video**

https://ieeexplore.ieee.org/document/6406936

·Developing evasive action-based indicators for identifying pedestrian conflicts in less organized traffic environments

·**Sparse reconstruction cost for abnormal event detection ***

https://ieeexplore.ieee.org/document/5995434

·Abnormal event detection at 150 fps in matlab

·Learning temporal regularity in video sequences

·**Abnormal event detection in videos using spatiotemporal autoencoder**

https://link.springer.com/chapter/10.1007/978-3-319-59081-3_23

·Future frame prediction for anomaly detection–a new baseline.

·A revisit of sparse coding based anomaly detection in stacked rnn framework

·**Anomaly detection in crowded scenes**

https://ieeexplore.ieee.org/document/5539872

·Joint detection and recounting of abnormal events by learning deep generic knowledge

·Anomaly detection in video using predictive convolutional long short-term memory networks

https://arxiv.xilesou.top/abs/1612.00390.pdf

·**Online detection of unusual events in videos via dynamic sparse coding**

https://ieeexplore.ieee.org/document/5995524

·**A review of anomaly detection in automated surveillance**

https://ieeexplore.ieee.org/document/6392472

·**An overview of deep learning based methods for unsupervised and semi-supervised anomaly detection in videos**

https://www.mdpi.com/2313-433X/4/2/36

·**Adversarial autoencoders for anomalous event detection in images**

https://scholarworks.iupui.edu/handle/1805/12352

·**Real-time video analysis on an embedded smart camera for traffic surveillance.**

https://ieeexplore.ieee.org/document/1317262

·**Video anomaly detection using deep incremental slow feature analysis network**

https://digital-library.theiet.org/content/journals/10.1049/iet-cvi.2015.0271

**scene modeling**

Learning semantic scene models by trajectory analysis

Learning object motion patterns for anomaly detection and improved object detection

Unsupervised learning of functional categories in video scenes

Scene Modeling-based Anomaly Detection for Intelligent Transport System

Video scene understanding using multi-scale analysis

Textures of optical flow for real-time anomaly detection in crowds





