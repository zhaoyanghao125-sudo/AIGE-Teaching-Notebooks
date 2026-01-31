# AlphaFold2 蛋白质结构预测

## 简介

使用 ColabFold v1.5.5 进行蛋白质三维结构预测，基于 AlphaFold2 和 MMseqs2。

## 功能

-  单体蛋白结构预测
-  复合物/多聚体结构预测（用 `:` 分隔链）
-  可选 Amber 结构松弛
-  支持 PDB100 模板或自定义模板

## 运行环境

- Google Colab（需要 GPU，推荐 A100）
- Python 3.x

## 快速开始

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/zhaoyanghao125-sudo/AIGE-Teaching-Notebooks/blob/main/01-AlphaFold2蛋白质/中文教学版AlphaFold2.ipynb)

1. 点击上方按钮在 Colab 中打开
2. 输入蛋白质氨基酸序列
3. 点击 **运行时 → 全部运行**
4. 等待预测完成，下载结果

## 示例输入
```
# 单体（溶菌酶）
KVFGRCELAAAMKRHGLDNYRGYSLGNWVCAAKFESNFNTQATNRNTDGSTDYGILQINSRWWCNDGRTPGSRNLCNIPCSALLSSDITASVNCAKKIVSDGNGMNAWVAWRNRCKGTDVQAWIRGCRL

# 复合物（用冒号分隔）
SEQ_A:SEQ_B
```

## 输出结果

- PDB 格式结构文件
- 模型质量图（pLDDT）
- MSA 覆盖度图
- PAE 预测对齐误差图

## 参考文献

- [ColabFold: Making protein folding accessible to all (Nature Methods, 2022)](https://www.nature.com/articles/s41592-022-01488-1)
- [AlphaFold2 (Nature, 2021)](https://www.nature.com/articles/s41586-021-03819-2)
