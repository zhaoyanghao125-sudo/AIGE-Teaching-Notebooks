# AIGE AI+学科实验设计

本仓库包含19个AI+学科交叉教学案例，涵盖生物、化学、物理、数学、天文、文史等领域。

## 案例目录

| 序号 | 主题 | 学科领域 |
|------|------|----------|
| 01 | AlphaFold2 蛋白质结构预测 | 生物 |
| 02 | 基因海洋 GeneSearch | 生物 |
| 03 | AlphaGeometry 几何证明 | 数学 |
| 04 | DeepSeek 数学证明 | 数学 |
| 05 | AI 数学猜想 | 数学 |
| 06 | AI 发现物理规律 | 物理 |
| 07 | AI 原子间作用力 | 物理/化学 |
| 08 | AI 探索酶特异性 | 生物/化学 |
| 09 | GT4SD 设计新分子 | 化学 |
| 10 | GraphCast 天气预测 | 地球科学 |
| 11 | AI 气候预测 LSTM | 地球科学 |
| 12 | AI 发现海洋垃圾 | 环境科学 |
| 13 | AI 识别星系形态 | 天文 |
| 14 | AI 重建古籍残片 | 文史 |
| 15 | AI 识别生成甲骨文 | 文史 |
| 16 | AI 修复文物残片 | 文史 |
| 17 | AI 校勘古籍 | 文史 |
| 18 | AI 重构唐诗分析 | 文史 |
| 19 | AI 解析文化融合 | 文史 |

## 使用方法

### 方法一：Colab 打开（推荐）

点击进入对应目录，然后用以下格式在 Colab 打开：
```
https://colab.research.google.com/github/zhaoyanghao125-sudo/AIGE-Teaching-Notebooks/blob/main/目录名/文件名.ipynb
```

### 方法二：本地运行
```bash
git clone https://github.com/zhaoyanghao125-sudo/AIGE-Teaching-Notebooks.git
cd AIGE-Teaching-Notebooks
jupyter notebook
```

## 说明

- 每个目录对应一个独立的教学案例
- 部分案例需要 GPU 运行环境
- 详细说明见各目录内的 README

---

## 开源声明与致谢

本仓库的教学案例使用了以下开源项目、模型和数据集，在此表示感谢：

### 模型与工具

| 项目 | 来源 | 许可证 |
|------|------|--------|
| AlphaFold2 | DeepMind | Apache 2.0 |
| GraphCast | Google DeepMind | Apache 2.0 |
| GT4SD | IBM Research | MIT |
| LightGlue | ETH Zurich (cvg) | Apache 2.0 |
| Aeneas/Ithaca | Google DeepMind | Apache 2.0 |
| HUST-OBC | 华中科技大学 | CC BY 4.0 |
| EZSpecificity | Nature 论文配套 | CC BY 4.0 |

### 数据集

| 数据集 | 来源 | 许可证 |
|--------|------|--------|
| MARIDA | Kikaki et al. (2022) | CC BY 4.0 |
| Galaxy Zoo 2 | Willett et al. (2013) | CC BY 4.0 |
| chinese-poetry | GitHub 开源 | MIT |
| CBDB | 哈佛/北大/中研院 | 学术使用 |
| ERA5 | ECMWF | Copernicus License |
| NASA GISTEMP | NASA GISS | Public Domain |

### 其他资源

- Sentence-Transformers (Apache 2.0)
- Hugging Face Transformers (Apache 2.0)
- PyTorch (BSD)
- RDKit (BSD)

## 使用须知

1. **教学用途**：本仓库内容仅供教学和学术研究使用
2. **引用要求**：如在论文或项目中使用，请引用原始数据集和模型的相关论文
3. **许可证遵守**：使用时请遵守各项目的原始许可证条款

## 许可证

本项目采用 [MIT License](LICENSE) 开源许可证。

---

*AIGE中心 AI+学科实验设计*
