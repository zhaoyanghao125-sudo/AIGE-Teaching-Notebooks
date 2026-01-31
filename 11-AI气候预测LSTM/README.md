# AI 气候预测：用神经网络预测地球的未来

## 简介

基于 LSTM 深度学习模型的全球气温趋势预测实验，体验如何使用人工智能分析历史气候数据并预测未来趋势。

## 学习内容

1. 气候数据的获取与可视化
2. LSTM神经网络如何学习时间序列规律
3. 亲手训练一个AI气候预测模型
4. 交互式实验：调整参数，观察不同情景下的未来气候
5. 探索家乡：查看中国各城市的气候变化趋势

## 什么是LSTM？

| 特性 | 说明 |
|------|------|
| 全称 | 长短期记忆网络 (Long Short-Term Memory) |
| 类型 | 循环神经网络 (RNN) 的改进版本 |
| 特长 | 学习时间序列数据中的长期依赖关系 |
| 应用 | 股票预测、天气预报、语音识别、气候建模 |

## 数据来源

本实验使用 NASA GISS（戈达德太空研究所）提供的全球地表温度数据集 (GISTEMP)，这是全球最权威的气候数据之一。

## 运行环境

- Google Colab（推荐 GPU）
- TensorFlow 2.x
- pandas、matplotlib、ipywidgets

## 快速开始

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/zhaoyanghao125-sudo/AIGE-Teaching-Notebooks/blob/main/11-AI气候预测LSTM/AI气候预测LSTM.ipynb)

1. 点击上方按钮在 Colab 中打开
2. 切换到 GPU 运行时（可选，加速训练）
3. 运行环境配置
4. 下载 NASA 气候数据
5. 训练 LSTM 模型并进行预测

## 实验内容

| 部分 | 内容 |
|------|------|
| 第零部分 | 环境配置与准备 |
| 第一部分 | 气候数据探索 |
| 第二部分 | 理解AI如何学习 |
| 第三部分 | 训练你的AI气候模型 |
| 第四部分 | 预测未来气候 |
| 第五部分 | 探索中国城市气候 |
| 第六部分 | 多情景对比与思考 |

## 交互式参数

| 参数 | 说明 | 范围 |
|------|------|------|
| CO2 年增长率 | 二氧化碳排放增长速度 | 0-5% |
| 减排起始年份 | 开始减排的年份 | 2025-2060 |
| 预测终止年份 | 预测到哪一年 | 2050-2150 |

## 预测情景示例

- 当前温度异常: 1.19C
- 2110年预测温度异常: 1.69C
- 预计升温幅度: +0.51C

## 1.5C 控制目标说明

超过 1.5C 意味着：
- 热浪更加频繁
- 珊瑚礁灭绝风险增加
- 部分低洼地区面临洪水威胁

## 参考资料

- [NASA GISS 温度数据](https://data.giss.nasa.gov/gistemp/)
- [LSTM 原理介绍](https://colah.github.io/posts/2015-08-Understanding-LSTMs/)
- [TensorFlow 官方文档](https://www.tensorflow.org/)
