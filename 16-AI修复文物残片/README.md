# AI 拼接与修复文物残片：用深度学习重建人类文明记忆

## 简介

基于深度学习特征匹配（SuperPoint + LightGlue）和边缘像素相似度算法的文物碎片自动拼接实验。

## 学习内容

1. 碎片数据的生成与可视化
2. 深度学习特征匹配（SuperPoint + LightGlue）如何找到图像对应关系
3. 边缘像素相似度算法如何自动拼接碎片
4. 可视化探索：观察AI如何"思考"匹配问题
5. 对比实验：传统方法 vs 深度学习方法

> **说明**：本实验中，LightGlue 用于**演示和理解**特征匹配原理，实际的碎片拼接使用更简单高效的**边缘像素相似度**算法。

## 什么是 LightGlue？

| 特性 | 说明 |
|------|------|
| 全称 | 轻量级特征匹配网络 (Light Glue Network) |
| 类型 | 基于Transformer的深度特征匹配器 |
| 特长 | 快速、准确地找到两张图像中的对应点 |
| 应用 | 3D重建、视觉定位、文物修复、图像拼接 |

## 核心技术

| 技术 | 作用 | 特点 |
|------|------|------|
| SuperPoint | 特征提取 | 自监督学习，鲁棒性强 |
| LightGlue | 特征匹配 | 基于Transformer，速度快 |
| 相似度矩阵 | 关系建模 | 量化碎片间的匹配程度 |
| 贪心算法 | 拼接决策 | 简单有效，可扩展 |

## 运行环境

- Google Colab（推荐 GPU）
- PyTorch
- LightGlue
- OpenCV

## 快速开始

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/zhaoyanghao125-sudo/AIGE-Teaching-Notebooks/blob/main/16-AI修复文物残片/AI碎片修复.ipynb)

1. 点击上方按钮在 Colab 中打开
2. 切换到 GPU 运行时（加速推理）
3. 运行环境配置
4. 生成模拟碎片数据
5. 体验 AI 特征匹配与自动拼接

## 实验内容

| 部分 | 内容 |
|------|------|
| 第零部分 | 环境配置与准备 |
| 第一部分 | 生成模拟碎片数据 |
| 第二部分 | 理解AI特征提取 |
| 第三部分 | 深度学习特征匹配 |
| 第四部分 | 自动拼接碎片 |
| 第五部分 | 真实文物碎片挑战 |
| 第六部分 | 可视化与3D展示 |

## 术语表

| 术语 | 英文 | 解释 |
|------|------|------|
| 特征点 | Keypoint | 图像中具有独特性的点 |
| 描述子 | Descriptor | 描述特征点周围区域的向量 |
| 内点 | Inlier | 通过几何验证的正确匹配 |
| 外点 | Outlier | 错误的匹配（误匹配） |
| RANSAC | - | 随机采样一致性算法 |
| 单应性矩阵 | Homography | 描述两个平面间变换关系的矩阵 |

## AI 的优势与局限

**优势：**
- 速度快：毫秒级完成匹配
- 一致性：不受疲劳影响，结果可复现
- 可扩展：能处理大规模碎片集

**局限：**
- 缺乏常识：不理解图像内容的语义
- 依赖纹理：纯色区域特征点少
- 需要人工：最终判断仍需专家确认

## 参考资源

- [LightGlue GitHub](https://github.com/cvg/LightGlue)
- [SuperPoint 论文 (CVPR 2018)](https://arxiv.org/abs/1712.07629)
- [RePAIR 数据集](https://zenodo.org/records/13993089)
- [Image Matching WebUI](https://github.com/Vincentqyw/image-matching-webui)
