# AI 识别甲骨文：用神经网络解读三千年前的文字

## 简介

基于 ResNet50 深度学习模型的甲骨文字符识别实验，体验如何使用人工智能识别中国最古老的成熟文字——甲骨文。

## 学习内容

1. 甲骨文数据集的结构与可视化
2. 卷积神经网络如何学习图像特征
3. 加载预训练模型进行文字识别
4. 批量测试：验证AI的识别准确率
5. 深入分析：探索AI的成功与失败案例

## 什么是甲骨文？

| 特性 | 说明 |
|------|------|
| 年代 | 约公元前1300年-公元前1046年（商朝晚期） |
| 载体 | 龟甲、兽骨 |
| 用途 | 占卜记录 |
| 发现 | 1899年，河南安阳殷墟 |
| 数量 | 已发现约15万片，含4500余单字 |
| 解读 | 已识别约1500字，仍有大量未解读 |

## 数据集与模型

本实验使用 HUST-OBC 教学精简版：

| 资源 | 说明 |
|------|------|
| 数据集 | 150个字符类别，1200张图片（5.4 MB） |
| 模型 | ResNet50 预训练权重（204 MB） |
| 准确率 | 94.6%（完整数据集测试结果） |

完整数据集（1588个字符类别，14万张图片）：
- [官方GitHub](https://github.com/Pengjie-W/HUST-OBC)
- [Figshare下载](https://figshare.com/s/8a9c0420312d94fc01e3)

## 运行环境

- Google Colab（推荐 GPU）
- PyTorch
- torchvision

## 快速开始

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/zhaoyanghao125-sudo/AIGE-Teaching-Notebooks/blob/main/15-AI识别甲骨文/AI识别甲骨文.ipynb)

1. 点击上方按钮在 Colab 中打开
2. 切换到 GPU 运行时（加速推理）
3. 运行环境配置
4. 下载数据集和预训练模型
5. 进行甲骨文识别实验

## 实验内容

| 部分 | 内容 |
|------|------|
| 第零部分 | 环境配置与准备 |
| 第一部分 | 认识甲骨文数据集 |
| 第二部分 | 理解AI如何识别文字 |
| 第三部分 | 加载预训练模型 |
| 第四部分 | 甲骨文识别实验 |
| 第五部分 | 深入探索与分析 |
| 第六部分 | 总结与思考 |

## 模型架构

- 基础模型：ResNet50
- 输入：224×224 灰度图像
- 输出：150个字符类别的概率分布
- 训练数据：HUST-OBC 数据集

## 参考文献

Wang P, Zhang K, Wang X, et al. An open dataset for oracle bone script recognition and decipherment. *Scientific Data*, 2024.
