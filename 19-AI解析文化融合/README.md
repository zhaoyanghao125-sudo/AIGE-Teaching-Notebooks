# AI 解读民国文学：古典与现代的文化融合分析

## 简介

基于深度学习的民国作家风格识别与文化成分研究，体验如何使用 AI 分析文学作品，探索作家风格与中西文化融合的规律。

## 学习内容

1. 了解文本向量化技术如何将文学作品转化为数学表示
2. 体验猜作家游戏：AI能否准确识别不同作家的风格？
3. 掌握文化成分分析：量化文本中的古典与现代元素
4. 探索风格空间可视化：在二维平面上看清作家之间的风格距离
5. 使用AI解说员：让大语言模型解读风格差异的文化原因
6. 尝试AI模仿作家：生成特定作家风格的文字

## 数据来源

| 数据集 | 来源 | 用途 |
|--------|------|------|
| luxun | GitHub开源项目 | 鲁迅全集（呐喊、彷徨、野草等） |
| literature-books | GitHub开源项目 | 老舍、周作人、季羡林等作家作品 |
| chinese-poetry | GitHub开源项目 | 论语、诗经（古典文言参照） |

## 研究维度

- **古典性**：文言词汇占比、古典意象使用频率
- **现代性**：白话程度、外来概念词汇占比
- 本实验聚焦于探索民国作家如何在传统与现代之间寻找平衡

## 收录作家

| 作家 | 代表作品 | 风格特点 |
|------|----------|----------|
| 鲁迅 | 呐喊、彷徨、野草 | 犀利、深刻、批判性强 |
| 老舍 | 骆驼祥子、茶馆 | 京味浓厚、幽默讽刺 |
| 周作人 | 散文集 | 平淡冲和、知识性强 |
| 季羡林 | 散文集 | 学者风范、融贯中西 |
| 论语 | 古典参照 | 文言文典范 |

## 运行环境

- Google Colab（推荐 GPU，A100 最佳）
- sentence-transformers
- transformers、accelerate（用于 AI 模仿作家）
- jieba、plotly、gradio

## 快速开始

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/zhaoyanghao125-sudo/AIGE-Teaching-Notebooks/blob/main/19-AI解析文化融合/AI解读文学.ipynb)

1. 点击上方按钮在 Colab 中打开
2. 切换到 GPU 运行时（推荐 A100）
3. 运行环境配置
4. 下载民国文学数据集
5. 体验作家风格分析与 AI 模仿

## 实验内容

| 部分 | 内容 |
|------|------|
| 第零部分 | 环境配置与准备 |
| 第一部分 | 数据下载与加载 |
| 第二部分 | 数据探索与预处理 |
| 第三部分 | AI文本向量化 |
| 第四部分 | 猜作家游戏 |
| 第五部分 | 文化成分分析仪 |
| 第六部分 | 风格空间可视化 |
| 第七部分 | 作家风格热力图 |
| 第八部分 | AI风格解说员 |
| 第九部分 | AI模仿作家 |

## 功能亮点

### 猜作家游戏
输入一段文字，AI 根据风格特征猜测是哪位作家写的。

### 文化成分分析仪
量化分析文本中的古典元素与现代元素占比，生成可视化雷达图。

### 风格空间可视化
使用 UMAP 降维，在二维平面上展示不同作家的风格距离。

### AI 模仿作家
使用大语言模型，模仿特定作家的风格生成新的文字。

## 核心技术

| 技术 | 作用 |
|------|------|
| Sentence-Transformers | 文本向量化 |
| UMAP | 高维降维可视化 |
| Cosine Similarity | 风格相似度计算 |
| jieba | 中文分词 |
| Transformers | AI 文本生成 |

## 参考资源

- [鲁迅全集 GitHub](https://github.com/Ac-heron/luxun)
- [Sentence-Transformers](https://www.sbert.net/)
- [Hugging Face Transformers](https://huggingface.co/docs/transformers)
