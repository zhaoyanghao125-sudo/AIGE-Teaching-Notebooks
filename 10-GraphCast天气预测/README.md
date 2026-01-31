# GraphCast：AI 预测天气

## 简介

基于 Google DeepMind 论文《Learning skillful medium-range global weather forecasting》(Science, 2023)，体验如何使用图神经网络进行全球天气预测。

## GraphCast 简介

| 特性 | 说明 |
|------|------|
| 开发者 | Google DeepMind |
| 发表 | Science, 2023 |
| 分辨率 | 0.25度（约28km） |
| 预测范围 | 10天 |
| 推理速度 | <1分钟（单次10天预测） |
| 核心技术 | 图神经网络（GNN） |

GraphCast 在超过 90% 的评估指标上超越了传统数值天气预报（NWP）系统 HRES。

## 学习内容

1. 天气数据的基本结构与探索方法
2. 图神经网络 (GNN) 在气象预测中的应用原理
3. GraphCast 模型的加载与推理
4. 可视化预测结果（全球与中国区域）
5. 参数实验与误差分析

## 运行环境

- Google Colab（需要 GPU）
- 推荐：A100 / V100 / T4
- 显存：>=16GB（推荐40GB+）

## 快速开始

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/zhaoyanghao125-sudo/AIGE-Teaching-Notebooks/blob/main/10-GraphCast天气预测/GraphCast天气预测.ipynb)

1. 点击上方按钮在 Colab 中打开
2. 切换到 GPU 运行时（推荐 A100）
3. 运行环境配置（安装 GraphCast 和依赖）
4. 下载预训练模型和样例数据
5. 运行预测并可视化结果

## 实验内容

| 部分 | 内容 |
|------|------|
| 第零部分 | 环境配置 |
| 第一部分 | 天气数据探索 |
| 第二部分 | 图神经网络与GraphCast原理 |
| 第三部分 | 模型加载与预测 |
| 第四部分 | 预测结果可视化与分析 |
| 第五部分 | 参数实验 |
| 第六部分 | 总结与拓展 |

## 模型版本

| 模型 | 分辨率 | 气压层 | 说明 |
|------|--------|--------|------|
| GraphCast | 0.25度 | 37 层 | 完整版，需要大量显存 |
| GraphCast_small | 1.0度 | 13 层 | 轻量版，适合学习和实验 |
| GraphCast_operational | 0.25度 | 13 层 | 业务版 |

本实验使用 GraphCast_small，适合在 Colab 免费 GPU 上运行。

## 术语表

| 术语 | 解释 |
|------|------|
| ERA5 | ECMWF 第五代再分析数据集 |
| GNN | 图神经网络 |
| RMSE | 均方根误差 |
| NWP | 数值天气预报 |
| HRES | 高分辨率预报 |
| Autoregressive | 自回归，将预测结果作为下一步输入 |

## 参考资料

- [GraphCast 论文 (Science)](https://www.science.org/doi/10.1126/science.adi2336)
- [GraphCast GitHub](https://github.com/google-deepmind/graphcast)
- [Google DeepMind 博客](https://deepmind.google/discover/blog/graphcast-ai-model-for-faster-and-more-accurate-global-weather-forecasting/)
- [官方 Colab Demo](https://colab.research.google.com/github/google-deepmind/graphcast/blob/main/graphcast_demo.ipynb)
