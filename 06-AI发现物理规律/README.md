# PhyE2E：AI 发现物理规律

## 简介

基于 Nature Machine Intelligence 论文《A Neural Symbolic Model for Space Physics》，体验如何使用 AI 从观测数据中自动发现物理规律。

## 学习内容

1. 传统拟合方法的原理与局限性
2. 符号回归的核心思想
3. PhyE2E 模型的使用方法
4. 在真实物理数据上发现公式
5. 多种方法的对比分析

## 运行环境

- Google Colab（需要 GPU）
- 推荐 A100 GPU
- 模型文件约 356 MB

## 快速开始

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/zhaoyanghao125-sudo/AIGE-Teaching-Notebooks/blob/main/06-AI发现物理规律/PhyE2E_AI_发现物理规律.ipynb)

1. 点击上方按钮在 Colab 中打开
2. 切换到 GPU 运行时
3. 运行环境配置（克隆仓库、安装依赖、下载模型）
4. 选择预设数据或自定义公式进行实验

## 实验内容

| 部分 | 内容 |
|------|------|
| 第零部分 | 环境准备 |
| 第一部分 | 传统拟合方法 |
| 第二部分 | 符号回归介绍 |
| 第三部分 | PhyE2E 模型使用 |
| 第四部分 | 真实物理数据实验 |
| 第五部分 | 方法对比分析 |
| 第六部分 | 自主实验区 |

## 预设数据类型

| 类型 | 公式 | 适用场景 |
|------|------|----------|
| linear | y = 2x + 3 | 线性关系 |
| quadratic | y = x² - 2x + 1 | 二次函数 |
| trig | y = sin(x) + 0.5x | 三角函数 |
| freefall | y = 0.5gx² | 自由落体 |
| exponential | y = e^(0.3x) | 指数增长 |

## 自定义公式写法

| 数学表达式 | 代码写法 |
|-----------|---------|
| x² + 2x + 1 | `x**2 + 2*x + 1` |
| sin(x) | `np.sin(x)` |
| e^x | `np.exp(x)` |
| ln(x) | `np.log(x)` |

## 术语表

| 术语 | 解释 |
|------|------|
| 符号回归 | 从数据中发现数学公式 |
| MCTS | 蒙特卡洛树搜索 |
| GP | 遗传编程 |
| Transformer | 一种神经网络架构 |

## 参考文献

- [论文原文 (Nature Machine Intelligence)](https://www.nature.com/articles/s42256-025-01126-3)
- [arXiv 预印本](https://arxiv.org/abs/2503.07994)
- [GitHub 仓库](https://github.com/Jie0618/PhysicsRegression)
