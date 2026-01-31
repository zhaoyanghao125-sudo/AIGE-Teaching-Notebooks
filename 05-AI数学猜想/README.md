# PySR 符号回归：让 AI 发现数学公式

## 简介

体验人工智能的"数学直觉"——让 AI 从数据中自动发现数学公式，而不是给出黑箱模型。

## 什么是符号回归？

| 方法 | 输出 | 可解释性 |
|------|------|----------|
| 神经网络 | 一堆权重数字 | 黑箱 |
| 符号回归 | 数学公式 | 完全透明 |

## 什么是 PySR？

PySR 是目前最强大的开源符号回归工具之一，由剑桥大学开发。

| 特性 | 说明 |
|------|------|
| 算法 | 遗传算法 + 模拟退火 |
| 后端 | Julia（高性能） |
| 接口 | Python（易用） |
| 论文 | arXiv:2305.01582 |

## 运行环境

- Google Colab
- Python 3.x
- 首次运行需安装 Julia 后端（约 3-5 分钟）

## 快速开始

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/zhaoyanghao125-sudo/AIGE-Teaching-Notebooks/blob/main/05-AI数学猜想/PySR数学发现.ipynb)

1. 点击上方按钮在 Colab 中打开
2. 运行环境配置（安装 PySR）
3. 选择要发现的公式类型
4. 观察 AI 如何从数据中发现数学规律

## 实验内容

| 部分 | 内容 | 预计时间 |
|------|------|----------|
| 第一部分 | 环境配置 | 3-5 分钟 |
| 第二部分 | 入门：发现简单公式 | 5 分钟 |
| 第三部分 | 进阶：发现物理定律 | 10 分钟 |
| 第四部分 | 挑战：费曼物理方程 | 15 分钟 |

## 可发现的公式示例

- 平方关系：y = x²
- 圆的面积：A = πr²
- 球的体积：V = (4/3)πr³
- 动能公式：E = (1/2)mv²
- 万有引力：F = Gm₁m₂/r²

## 核心参数

| 参数 | 说明 | 建议值 |
|------|------|--------|
| `niterations` | AI 搜索公式的轮数 | 简单 20-40，复杂 60-100 |
| `binary_operators` | 二元运算符 | +, -, *, / |
| `unary_operators` | 一元运算符 | sin, cos, square, cube |

## 参考资料

- [PySR 官方文档](https://github.com/MilesCranmer/PySR)
- [PySR 论文 (arXiv:2305.01582)](https://arxiv.org/abs/2305.01582)
- [费曼符号回归数据库](https://space.mit.edu/home/tegmark/aifeynman.html)
