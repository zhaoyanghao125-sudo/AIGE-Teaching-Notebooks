# AI 识别星系形态：用深度学习探索宇宙

## 简介

基于卷积神经网络(CNN)的星系图像自动分类，体验如何使用人工智能自动识别不同类型的星系。

## 学习内容

1. 星系形态的基本知识（螺旋星系、椭圆星系、不规则星系）
2. 卷积神经网络 (CNN) 如何"看懂"图像
3. 迁移学习：站在巨人肩膀上训练AI
4. 亲手训练一个星系分类模型
5. 可视化分析：理解AI的判断依据

## 什么是卷积神经网络(CNN)？

| 特性 | 说明 |
|------|------|
| 全称 | 卷积神经网络 (Convolutional Neural Network) |
| 类型 | 深度学习模型，专门处理图像数据 |
| 特长 | 自动提取图像特征，识别物体形状、纹理、结构 |
| 应用 | 人脸识别、医学影像、自动驾驶、天文图像分析 |

## 星系分类

| 类别 | 英文 | 特征 |
|------|------|------|
| 螺旋星系 | Spiral | 具有明显旋臂结构 |
| 椭圆星系 | Elliptical | 呈椭圆形，无明显结构 |
| 不规则星系 | Irregular | 形状不规则 |

## 数据来源

本实验使用 Galaxy Zoo 2 项目的公开数据集，这是一个由数十万名公民科学家参与的星系分类项目。

- 图片来源：[Zenodo](https://zenodo.org/records/3565489)
- 标签来源：[Galaxy Zoo Data](https://data.galaxyzoo.org)
- 许可证：CC BY 4.0

## 运行环境

- Google Colab（推荐 GPU）
- TensorFlow 2.x
- pandas、matplotlib、seaborn

## 快速开始

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/zhaoyanghao125-sudo/AIGE-Teaching-Notebooks/blob/main/13-AI识别星系/AI识别星系.ipynb)

1. 点击上方按钮在 Colab 中打开
2. 切换到 GPU 运行时（加速训练）
3. 运行环境配置
4. 下载星系图像数据
5. 训练 CNN 模型并进行分类

## 实验内容

| 部分 | 内容 |
|------|------|
| 第零部分 | 环境配置与数据准备 |
| 第一部分 | 认识星系 |
| 第二部分 | 数据预处理 |
| 第三部分 | 构建AI分类器 |
| 第四部分 | 训练模型 |
| 第五部分 | 评估与可视化 |
| 第六部分 | 自己动手试一试 |

## 模型架构

- 预训练模型：MobileNetV2（迁移学习）
- 自定义分类头：GlobalAveragePooling2D + Dense + Dropout
- 优化器：Adam
- 损失函数：Categorical Crossentropy

## 评估指标

- 混淆矩阵
- 分类报告（Precision, Recall, F1-Score）
- 准确率曲线

## 思考题

1. 为什么螺旋星系和椭圆星系有时会被混淆？
2. 如果要提高不规则星系的识别准确率，可以采取哪些措施？
3. AI分类与人类分类相比，有哪些优势和不足？

## 参考文献

Willett, K. W., et al. (2013). Galaxy Zoo 2: detailed morphological classifications for 304,122 galaxies from the Sloan Digital Sky Survey. MNRAS, 435(4), 2835-2860.
