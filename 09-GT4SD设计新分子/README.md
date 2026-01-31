# GT4SD：AI 分子设计实验

## 简介

基于 IBM GT4SD (Generative Toolkit for Scientific Discovery) 平台，体验 AI 驱动的分子设计完整流程。

## 学习内容

1. 分子表示：学习 SMILES 字符串的基本概念
2. AI 分子生成：体验 AI 模型生成新分子
3. 分子可视化：将 SMILES 转换为 2D/3D 结构图
4. 性质计算：预测分子的物理化学性质
5. 药物评估：Lipinski 规则与 QED 分数

## 技术栈

| 工具 | 用途 |
|------|------|
| GT4SD | AI 分子生成框架 |
| RDKit | 分子处理、可视化、性质计算 |
| py3Dmol | 3D 分子可视化 |

## 运行环境

- Google Colab
- 需要安装 Miniconda（Python 3.10）
- RDKit 用于分子处理

## 快速开始

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/zhaoyanghao125-sudo/AIGE-Teaching-Notebooks/blob/main/09-GT4SD设计新分子/GT4SD.ipynb)

1. 点击上方按钮在 Colab 中打开
2. 运行环境配置（安装 Miniconda 和 RDKit）
3. 学习 SMILES 分子表示
4. 体验 AI 分子生成
5. 分析分子性质

## 实验内容

| 部分 | 内容 |
|------|------|
| 第零部分 | 环境准备 |
| 第一部分 | SMILES 基础 |
| 第二部分 | AI 分子生成 |
| 第三部分 | 分子可视化 |
| 第四部分 | 性质计算 |
| 第五部分 | 自由研究 |

## GT4SD 模型

| 模型 | 来源 | 功能 |
|------|------|------|
| T5 | GT4SD/multitask-text-and-chemistry | 文本到分子生成 |
| REINVENT | AstraZeneca | 基于 RNN 的分子生成 |
| Regression Transformer | GT4SD | 性质约束生成 |
| MoLeR | Microsoft | 基于骨架的分子生成 |
| TorchDrug | MIT | 药物发现分子生成 |

## 分子性质说明

| 性质 | 缩写 | Lipinski 规则 |
|------|------|---------------|
| 分子量 | MW | <= 500 |
| 脂水分配系数 | LogP | <= 5 |
| 氢键供体数 | HBD | <= 5 |
| 氢键受体数 | HBA | <= 10 |

## 参考资源

- [GT4SD GitHub](https://github.com/GT4SD/gt4sd-core)
- [GT4SD HuggingFace](https://huggingface.co/GT4SD)
- [GT4SD 论文 (Nature, 2023)](https://www.nature.com/articles/s41524-023-01028-1)
- [RDKit 文档](https://www.rdkit.org/docs/)
- [SMILES 教程](https://www.daylight.com/dayhtml/doc/theory/theory.smiles.html)
