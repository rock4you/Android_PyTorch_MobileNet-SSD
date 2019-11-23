# Android_PyTorch_MobileNet-SSD Pedestrian Detection
## 最终目标
实现一款能够在安卓手机上使用摄像头进行实时行人检测的软件。
## 技术方案：
使用PyTorch加载SSD预训练模型，在Caltech行人检测数据集上迁移学习；
使用PyTorch加载MobileNet-SSD预训练模型，在Caltech行人检测数据集上迁移学习；
编写安卓程序，分别加载上述两个模型，验证检测性能。

### 1.训练数据预处理
下载Caltech行人检测数据集：11个图像压缩包+1个标注文件压缩包

按照VOC格式提取并保存数据：

将seq转换为jpg

将vbb转为xml

将jpg和xml重命名

划分训练集、测试集

### 2.使用PyTorch加载SSD预训练模型，在Caltech行人检测数据集上迁移学习
