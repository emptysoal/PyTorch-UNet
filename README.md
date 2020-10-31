# PyTorch U-Net

## 简介

基于pytorch框架，构建UNet网络训练自己的数据集（鼠标和键盘图像数据集）进行语义分割。

## 文件说明

- self_data: 目录，存放着自己的用于训练和测试的数据集；
- test_result: 目录，用于存放推理（使用已训练好的模型预测）所得的结果；
- train_img: 目录，用于存放训练过程中的一些中间结果，可视化训练的程度；
- dataset.py: 读取数据集；
- unet.py: 搭建语义分割网络结构；
- train.py: 训练模型；
- predict.py: 使用训练好的模型进行推理

## 项目启动

### 训练模型

- 创建目录`models`，用于存放训练出的模型

```bash
mkdir models
```

- 开始训练，可进入`train.py`中修改超参数

```bash
python train.py
```

### 推理

- 运行`predict.py`，可进入`predict.py`中修改所用测试图片路径

```bash
python predict.py
```

