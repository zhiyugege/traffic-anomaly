# 知识图谱相关调研

|  ID  |             任务             |                             方法                             | cate |
| :--: | :--------------------------: | :----------------------------------------------------------: | ---- |
| P.1  |             分类             | 提出了Graph Search Neural Network (GSNN) ，利用importance net扩展邻居节点 | 显式 |
| P.2  |             动作             | 动作指令分解成And-Or grap，邻接矩阵表示后，编码成向量 LSTM训练 | 隐式 |
| P.3  |             VQA              | 对图谱中每对三元组（一个单元），word embedding+matrix，LSTM+attention | 隐式 |
| P.4  |        Image caption         |        word types and relation in KG embedding + LSTM        | 隐式 |
| P.5  |    scene graph generation    |    三元组 matrix based embedding encode by RNN+attention     | 隐式 |
| P.6  |      Zero-Shot Learning      | 由于存在祖先关系的节点信息传播有损失，提出DGP模块来挖掘图谱层次结构的信息 | 隐式 |
| P.7  |      Zero-Shot Learning      | Learning of the Propagation Matrix 来计算扩展时邻居节点的权重 | 隐式 |
| P.8  |    scene graph generation    | 目标是在场景图和常识图之间做实体和关系对齐，利用GGNN在节点间传播信息，计算相似度更新节点、边信息 | 显式 |
| P.9  | Zero-Shot Action Recognition | 知识图谱：word embedding+GCN  video features+GCN classification | 隐式 |
| P.10 |        HOI detection         |                   知识图谱 01 matrix + GCN                   | 隐式 |
| P.11 |    Relationship Detection    | 知识（关系的条件概率表示）作为teacher指导DNN由视觉特征生成的关系表示（条件概率），度量方式kl散度 | 隐式 |
| P.12 |    scene graph generation    |     根据数据集中的数据分布构建图谱（边信息为概率）+GGNN      | 隐式 |
| P.13 |             分类             | GGNN处理知识图谱，提出了门机制（attention）来对图像中与知识图谱中属性节点对应的区域激活 | 隐式 |
| P.14 |     relation extraction      | 利用toned-down graph edit distance来度量图谱间差异，指导实体和关系补全 | 显式 |
| P.15 |            RecSys            |    use TransE to learn embedding of entity&relation + GRU    | 隐式 |
| P.16 |            RecSys            |    use TransH to learn embedding of entity&relation + TUP    | 隐式 |
| P.17 |            RecSys            | learning the embedding of entity&relation + Collaborative Filtering | 隐式 |
| P.18 |            RecSys            | use TransR to learn embedding of entity&relation(structural) 、 textual 、visual features +Collaborative Filtering | 隐式 |
| P.19 |            RecSys            |       use TransR to learn embedding of entity&relation       | 隐式 |

|  ID  |                            文章名                            |   year   |
| :--: | :----------------------------------------------------------: | :------: |
| P.1  | The More You Know: Using Knowledge Graphs for Image Classiﬁcation | CVPR.17  |
| P.2  | Knowledge-guided recurrent neural network learning for task-oriented action prediction | ICME.17  |
| P.3  | Incorporating External Knowledge to Answer Open-Domain Visual Questions with Dynamic Memory Networks | CVPR.18  |
| P.4  |  Improving Image Captioning by Leveraging Knowledge Graphs   | arxiv.19 |
| P.5  | Scene Graph Generation with External Knowledge and Image Reconstruction | CVPR.19  |
| P.6  | Rethinking Knowledge Graph Propagation for Zero-Shot Learning | CVPR.19  |
| P.7  | Multi-Label Zero-Shot Learning with Structured Knowledge Graphs | CVPR.18  |
| P.8  |      Bridging Knowledge Graphs to Generate Scene Graphs      | arxiv.20 |
| P.9  | I Know the Relationships: Zero-Shot Action Recognition via Two-Stream Graph Convolutional Networks and Knowledge Graphs | AAAI.19  |
| P.10 | Learning to Detect Human-Object Interactions with Knowledge  | CVPR.19  |
| P.11 | Visual Relationship Detection with Internal and External Linguistic Knowledge Distillation | ICCV.17  |
| P.12 | Knowledge-Embedded Routing Network for Scene Graph Generation | CVPR.19  |
| P.13 | Knowledge-Embedded Representation Learning for Fine-Grained Image Recognition | CVPR.19  |
| P.14 | GREG: A Global Level Relation Extraction with Knowledge Graph Embedding |    -     |
| P.15 | Improving Sequential Recommendation with Knowledge-Enhanced Memory Networks | SIGIR.18 |
| P.16 | Unifying Knowledge Graph Learning and Recommendation: Towards a Better Understanding of User Preferences | arxiv.19 |
| P.17 |  Learning over Knowledge-Base Embeddings for Recommendation  | arxiv.18 |
| P.18 | Collaborative Knowledge Base Embedding for Recommender Systems |  KDD.16  |
| P.19 | Knowledge-based Recommendation with Hierarchical Collaborative Embedding | PAKDD.18 |
