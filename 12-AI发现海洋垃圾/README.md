# AI 发现海洋垃圾：用深度学习守护蓝色星球

## 简介

基于 Sentinel-2 卫星遥感与语义分割模型的海洋垃圾检测，体验如何使用人工智能分析卫星图像，自动检测海洋中的漂浮垃圾。

## 实验阶段

| 阶段 | 内容 | 数据 | 方法 |
|------|------|------|------|
| 第1-4部分 | 学习检测流程 | 模拟样本 | 光谱特征分析 |
| 第5部分 | 自主探索 | MARIDA真实数据 | U-Net++ AI模型 |

## 什么是语义分割?

| 特性 | 说明 |
|------|------|
| 定义 | 对图像中每个像素进行分类的技术 |
| 任务 | 识别图像中"什么东西在哪里" |
| 模型 | U-Net++ |
| 应用 | 医学影像、自动驾驶、卫星图像解译 |

## 数据与模型来源

| 组件 | 来源 | 说明 |
|------|------|------|
| 卫星数据 | MARIDA数据集 | 全球首个海洋垃圾遥感基准数据集 |
| 卫星平台 | Sentinel-2 (ESA) | 10米分辨率多光谱图像 |
| AI模型 | marinedebrisdetector | 基于U-Net++的专业检测器 |

## 运行环境

- Google Colab（推荐 GPU）
- PyTorch
- segmentation-models-pytorch
- rasterio

## 快速开始

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/zhaoyanghao125-sudo/AIGE-Teaching-Notebooks/blob/main/12-AI发现海洋垃圾/AI发现海洋垃圾.ipynb)

1. 点击上方按钮在 Colab 中打开
2. 切换到 GPU 运行时（可选）
3. 运行环境配置
4. 学习海洋垃圾检测流程
5. 使用真实 AI 模型进行检测

## 实验内容

| 部分 | 内容 |
|------|------|
| 第零部分 | 环境配置与准备 |
| 第一部分 | 认识海洋垃圾危机 |
| 第二部分 | 理解AI如何识别垃圾 |
| 第三部分 | AI检测海洋垃圾 (演示) |
| 第四部分 | 可视化与分析 |
| 第五部分 | 自主探索 (真实AI模型 + MARIDA数据) |
| 第六部分 | 总结与拓展 |

## 评估指标

| 指标 | 说明 |
|------|------|
| Precision | 精确率，检测结果中正确的比例 |
| Recall | 召回率，实际垃圾被检测到的比例 |
| F1 Score | 精确率和召回率的调和平均 |

## MARIDA 数据集

- 全球首个海洋垃圾遥感基准数据集
- 下载地址: https://doi.org/10.5281/zenodo.5151941
- 大小: 约1.2GB

## 参考文献

Kikaki K, et al. (2022) MARIDA: A benchmark for Marine Debris detection from Sentinel-2 remote sensing data. PLoS ONE 17(1): e0262247.
