# EZSpecificity：AI 探索酶的底物特异性

## 简介

基于 Nature 论文《Enzyme specificity prediction using cross-attention graph neural networks》，体验如何使用 AI 预测酶的底物特异性。

## 学习内容

1. 酶与底物的基础知识
2. 图神经网络如何表示分子
3. 交叉注意力机制如何捕捉酶-底物相互作用
4. 使用 EZSpecificity 进行底物预测
5. 分析模型的决策依据（Attention 可视化）

## 运行环境

- Google Colab（推荐 GPU）
- PyTorch + PyTorch Geometric
- RDKit（化学分子处理）
- Biopython（蛋白质序列处理）

## 快速开始

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/zhaoyanghao125-sudo/AIGE-Teaching-Notebooks/blob/main/08-AI探索酶特异性/EZSpecificity探索酶.ipynb)

1. 点击上方按钮在 Colab 中打开
2. 运行环境配置（安装依赖）
3. 下载数据和预训练模型（来自 Zenodo）
4. 体验酶-底物预测

## 数据来源

| 文件 | 大小 | 说明 |
|------|------|------|
| src.zip | 370 KB | 源代码 |
| saved_model.zip | 97 MB | 预训练权重 |
| data.zip | 459 MB | 数据集 |

- DOI: 10.5281/zenodo.17129895
- 许可证: CC-BY-4.0

## 实验内容

| 部分 | 内容 |
|------|------|
| 第零部分 | 环境准备 |
| 第一部分 | 认识数据 |
| 第二部分 | 引导式体验 |
| 第三部分 | 探索实验 |
| 第四部分 | 自由研究 |

## SMILES 格式示例
```
乙酸乙酯,CCOC(=O)C
乙酸甲酯,COC(=O)C
乙醇,CCO
苯甲酸甲酯,COC(=O)c1ccccc1
```

## 术语表

| 术语 | 英文 | 解释 |
|------|------|------|
| 酶 | Enzyme | 催化生化反应的蛋白质 |
| 底物 | Substrate | 酶作用的目标分子 |
| 特异性 | Specificity | 酶识别特定底物的能力 |
| 图神经网络 | GNN | 处理图结构数据的神经网络 |
| 注意力机制 | Attention | 让模型关注重要信息的机制 |
| SMILES | - | 用文本表示分子结构的方法 |

## 参考文献

- [论文原文 (Nature)](https://www.nature.com/articles/s41586-025-09697-2)
- [Zenodo 数据集](https://zenodo.org/records/17860476)
- [RDKit 文档](https://www.rdkit.org/docs/)
- [PyTorch Geometric 教程](https://pytorch-geometric.readthedocs.io/)
