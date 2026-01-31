# DeepSeek Prover V2：自动定理证明

## 简介

复现 DeepSeek 发布的 DeepSeek-Prover-V2 自动定理证明系统，使用大语言模型生成 Lean 4 形式化证明。

## 系统能力

- 理解数学定理的形式化表述
- 生成证明计划（Proof Plan），展示推理思路
- 输出可被 Lean 4 验证的完整证明代码

## 模型版本

| 组件 | 功能 | 本实验是否包含 |
|------|------|---------------|
| DeepSeek-Prover-V2-7B | 生成证明计划与 Lean 4 代码 | 包含 |
| DeepSeek-Prover-V2-671B | 更强的推理能力 | 不包含（需大量GPU）|
| Lean 4 + Mathlib | 形式化验证证明正确性 | 包含 |

## 运行环境

- Google Colab（需要 GPU，推荐 A100）
- 首次运行需下载约 14GB 模型

## 快速开始

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/zhaoyanghao125-sudo/AIGE-Teaching-Notebooks/blob/main/04-DeepSeek数学证明/Deepseek_prover.ipynb)

1. 点击上方按钮在 Colab 中打开
2. 运行环境配置（安装 Lean 4 和依赖）
3. 加载 7B 模型
4. 输入数学定理，生成证明

## 实验流程

1. 环境配置：安装 Lean 4、Mathlib、Python 依赖
2. 模型加载：加载 DeepSeek-Prover-V2-7B
3. 定理输入：输入 Lean 4 格式的定理声明
4. 证明生成：模型输出证明计划和代码
5. 形式化验证：使用 Lean 4 验证证明正确性

## 示例定理
```lean
-- 加法交换律
theorem add_comm (a b : Nat) : a + b = b + a := by
  sorry

-- 列表长度
theorem list_length_append (l1 l2 : List α) : 
  (l1 ++ l2).length = l1.length + l2.length := by
  sorry
```

## 注意事项

- 7B 模型对基础定理效果较好
- 复杂竞赛级题目可能需要多次重试
- Colab T4 GPU 可运行，A100 更快

## 参考资料

- [DeepSeek-Prover-V2 论文](https://arxiv.org/abs/2408.08152)
- [DeepSeek GitHub](https://github.com/deepseek-ai)
- [Lean 4 文档](https://lean-lang.org/)
