# AlphaGeometry：几何定理自动证明

## 简介

复现 DeepMind 在 Nature 2024 发表的 AlphaGeometry 系统中的 **DDAR 符号推理引擎**，体验 AI 如何自动证明国际数学奥林匹克（IMO）级别的几何题。

## 系统组成

| 组件 | 功能 | 本实验是否包含 |
|------|------|---------------|
| DDAR 符号推理引擎 | 基于规则的演绎推理 |  包含 |
| 语言模型 | 建议辅助构造点 |  不包含（需大量GPU）|

## 运行环境

- Google Colab（推荐 GPU）
- Python 3.10（会自动安装）

## 快速开始

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/zhaoyanghao125-sudo/AIGE-Teaching-Notebooks/blob/main/03-AlphaGeometry几何证明/AlphaGeometry.ipynb)

1. 点击上方按钮在 Colab 中打开
2. 运行环境配置（自动安装依赖）
3. 选择数据集（内置示例/AG-30/IMO题目）
4. 运行推理引擎，观察证明过程

## 数据集选项

| 选项 | 说明 | 适用场景 |
|------|------|----------|
| 内置示例 | 5道经典几何定理 | 快速验证、教学演示 |
| AG-30 | 论文官方测试集（30题）| 复现论文结果 |
| IMO-2000-2022 | 更大的IMO题目集合 | 深入研究 |
| 自定义上传 | 上传自己的题目 | 测试特定题目 |

## 题目格式示例
```
# 中点定理
a b c = triangle a b c; m = midpoint m a b; n = midpoint n a c ? para m n b c

# 垂心性质
a b c = triangle a b c; d = on_tline d b a c, on_tline d c a b ? perp a d b c

# 外心性质
a b c = triangle a b c; o = circumcenter o a b c ? cong o a o b
```

## 常用构造函数

| 函数 | 含义 |
|------|------|
| `triangle a b c` | 三角形ABC |
| `midpoint m a b` | M是AB的中点 |
| `incenter i a b c` | 内心 |
| `circumcenter o a b c` | 外心 |
| `foot d p a b` | D是P到AB的垂足 |

## 常用证明目标

| 谓词 | 含义 |
|------|------|
| `perp a b c d` | AB ⊥ CD |
| `para a b c d` | AB ∥ CD |
| `cong a b c d` | AB = CD |
| `coll a b c` | 三点共线 |

## 参考文献

- [Solving olympiad geometry without human demonstrations (Nature, 2024)](https://www.nature.com/articles/s41586-023-06747-5)
- [AlphaGeometry GitHub](https://github.com/google-deepmind/alphageometry)
