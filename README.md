# Anomaly-Detection

## 第一部分：无监督异常检测
### 1. 算法
#### 1.1 算法一：Isolation Forest
- 算法论文
- 算法解读
- 算法实现

#### 1.2 算法二：基于PCA的重构误差
- 算法论文
- 算法解读
- 算法实现

### 2. 性能对比
#### 2.1 选取的无监督异常检测算法
- Isolation Forest
- Local Outlier Factor 
- 基于KernelPCA的重构误差
- 基于LinearPCA的重构误差
- RobustPCC
- Mahalabonas Distance

#### 2.2 对比方案与数据集
- 以Isolation Forest为BaseLine
- 

#### 2.3 对比结论
- 一般来说，基于KernelPCA的重构误差**优于**基于LinearPCA的重构误差
- **对比代码：** [unsupervised_detection_contrast](https://github.com/Albertsr/Anomaly-Detection/blob/master/Algo%20Contrast/unsupervised_detection_contrast.py)
- **对比Jupyter Notebook：** [unsupervised_detection_contrast_jupyter](https://github.com/Albertsr/Anomaly-Detection/blob/master/Algo%20Contrast/%E6%97%A0%E7%9B%91%E7%9D%A3%E5%BC%82%E5%B8%B8%E6%A3%80%E6%B5%8B-%E7%AE%97%E6%B3%95%E5%AF%B9%E6%AF%94.ipynb)

![contra_pcc](https://github.com/Albertsr/Anomaly-Detection/blob/master/Algo%20Contrast/U_contra_pcc.jpg)

---

## 第二部分：半监督异常检测
### 1. 算法
#### 1.1 算法一：ADOA
- 算法论文
- 算法解读
- 算法实现

#### 1.2 算法一：PU Learning
- 算法论文
- 算法解读
- 算法实现


### 2. 算法性能对比
#### 2.1 验证思路与代码
- **思路**
  - U集中的正常样本服从正态分布
  - 已观测到的P集，以及U中混杂的异常样本由指数分布、伽马分布、卡方分布组合而成
  
- **代码**
  - [semi_contrast](https://github.com/Albertsr/Anomaly-Detection/blob/master/Algo%20Contrast/semi_contrast.py)

#### 2.2 对比结果
- 结果
  
  ![semi_contra](https://github.com/Albertsr/Anomaly-Detection/blob/master/Algo%20Contrast/semi_contra.jpg)
   
