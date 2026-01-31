# 探索基因的海洋：迷你序列搜索引擎（GeneSearch Lab）

## 简介

基于 Nature（2025）论文 "Efficient and accurate search in petabase-scale sequence repositories"，体验将海量序列库做成可检索搜索引擎的核心思想。

## 学习目标

-  **特征化（k-mer）**：将 DNA 序列切成可检索的短片段
-  **索引（倒排表）**：建立 k-mer → 序列ID 的映射加速检索
-  **查询与判别**：计算命中比例并用阈值过滤
-  **误差分析**：通过点突变实验观察 FP/FN 变化

## 运行环境

- Google Colab（支持 GPU 加速）
- Python 3.x

## 快速开始

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/zhaoyanghao125-sudo/AIGE-Teaching-Notebooks/blob/main/02-基因海洋GeneSearch/探索基因海洋GeneSearch_Lab.ipynb)

1. 点击上方按钮在 Colab 中打开
2. 输入要搜索的 DNA 片段（仅支持 A/C/G/T）
3. 设置参数（k-mer 长度、阈值等）
4. 点击 **运行时 → 全部运行**

## 核心参数

| 参数 | 说明 | 建议值 |
|------|------|--------|
| `k` | k-mer 长度（越大越精确，但对突变敏感） | 7/11/15 |
| `threshold` | 命中阈值（越高越严格） | 0.1/0.2/0.3 |
| `num_sequences` | 数据库序列条数 | 30-500 |
| `mutation_count` | 模拟突变数量 | 1-3 |

## 输出结果

- `db.fa`：模拟序列数据库
- `query.fa`：查询序列
- `result.csv`：候选序列得分
- `metrics.txt`：TP/FP/FN 指标
- `plots/*.png`：可视化图表

## 课堂建议

1. **第一次**：保持默认参数，跑通流程
2. **对比实验**：调整 k 值（7/11/15）观察 FP/FN 变化
3. **鲁棒性实验**：开启突变模式，观察检索准确率下降

## 参考文献

- [Efficient and accurate search in petabase-scale sequence repositories (Nature, 2025)](https://www.nature.com/articles/s41586-025-09603-w)
- [MetaGraph GitHub](https://github.com/ratschlab/metagraph)
