# AI 重建古籍残片：用神经网络复原历史文献

## 简介

基于 Google DeepMind Aeneas/Ithaca 项目的古代碑铭修复实验，体验人工智能如何"阅读"和"复原"古代文献。

## 学习内容

1. 古籍残片修复的挑战与传统人文学方法
2. Aeneas模型如何通过上下文学习自动修复拉丁文碑铭
3. 图像分析功能：上传碑铭照片，AI结合视觉特征进行修复
4. Ithaca模型如何处理古希腊文残卷
5. 通用语言模型（BERT）的填空原理演示
6. 对比分析专业模型与通用模型的差异

## 背景知识

| 概念 | 说明 |
|------|------|
| 碑铭学 (Epigraphy) | 研究古代刻写文字的学科 |
| 文本修复 (Restoration) | 补全残缺或损坏的文字 |
| 年代归属 (Dating) | 推断文献的书写年代 |
| 地理定位 (Attribution) | 确定文献的来源地区 |
| 平行文本 (Parallels) | 具有相似措辞或语境的其他文献 |
| 多模态分析 | 同时利用文本和图像信息进行推理 |

## 模型介绍

| 模型 | 语言 | 训练数据 |
|------|------|----------|
| Aeneas | 拉丁文 | 176,000+ 条罗马碑铭，支持图像输入 |
| Ithaca | 古希腊文 | 希腊碑铭数据库约 80,000 条碑铭 |

## 运行环境

- Google Colab（推荐 GPU）
- JAX（GPU版本）
- predictingthepast（DeepMind官方推理库）
- transformers（用于BERT演示）

## 快速开始

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/zhaoyanghao125-sudo/AIGE-Teaching-Notebooks/blob/main/14-AI重建古籍残片/AI修复文字残片.ipynb)

1. 点击上方按钮在 Colab 中打开
2. 切换到 GPU 运行时（加速推理）
3. 运行环境配置
4. 下载预训练模型
5. 体验古籍残片修复

## 实验内容

| 部分 | 内容 |
|------|------|
| 第零部分 | 环境配置与准备 |
| 第一部分 | 认识古籍残片 |
| 第二部分 | Aeneas模型 - 拉丁文碑铭修复 |
| 第三部分 | 图像分析与多模态修复 |
| 第四部分 | Ithaca模型 - 古希腊文残卷修复 |
| 第五部分 | BERT模型 - 通用语言填空原理 |
| 第六部分 | 模型对比与分析 |
| 第七部分 | 学生实验记录 |

## 示例

**拉丁文碑铭修复**
- 输入: `D M # IVLIO FORTVNATO`
- 修复: `D M S IVLIO FORTVNATO` (献给逝者尤利乌斯·福尔图纳图斯)

**古希腊文碑铭修复**
- 输入: `ΕΔΟΞΕΝ ΤΗΙ ΒΟΥΛΗΙ ΚΑΙ ΤΩΙ #`
- 修复: `ΕΔΟΞΕΝ ΤΗΙ ΒΟΥΛΗΙ ΚΑΙ ΤΩΙ ΔΗΜΩΙ` (议事会与人民决议)

## 参考资料

- [GitHub: predictingthepast](https://github.com/google-deepmind/predictingthepast)
- [Ithaca 在线演示](https://ithaca.deepmind.com)
- Assael et al. (2022) "Restoring and attributing ancient texts using deep neural networks" *Nature* 603, 280–283
- Sommerschield et al. (2023) "Machine learning for ancient languages: A survey" *Computational Linguistics*
