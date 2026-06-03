# 投研分析流程（Investment Research Workflow）

> 对每个 mega-trends 课题执行结构化多角色研究，模拟投行投研流程。
> 本目录存放流程定义、角色 prompt、输出模板。每次全量更新课题时按此流程执行。

## 目录结构

```
_research_workflow/
├── README.md           ← 你在这里（总览 + 使用方法）
├── workflow.md         ← 完整 7 轮流程（Agent 执行手册）
├── role_prompts.md     ← 7 个角色的系统 prompt 模板
└── output_format.md    ← 每轮的输出格式模板
```

## 使用方法

1. 选择要分析的课题编号（如 `07`）
2. 阅读本目录下全部 4 个文件
3. 按 `workflow.md` 中的 7 轮顺序执行
4. 每个角色的具体指令见 `role_prompts.md`
5. 每轮的输出格式见 `output_format.md`

## 角色总览

| 角色 | 代号 | 职责 | 启动轮次 |
|------|------|------|---------|
| 投资总监 | `cio` | 准备背景、假设框定、最终综合 | Round 0, 5 |
| 基本面研究员 | `fundamental` | 估值、财务、行业对比 | Round 1 |
| 催化剂研究员 | `catalyst` | 事件日历、监管、竞品、M&A | Round 1 |
| 宏观调研员 | `macro` | 利率/地缘/政策传导、风险因子 | Round 1 |
| 魔鬼辩护人 | `devil` | 系统性构建反方论据、寻找证伪 | Round 2 |
| 基金经理 | `pm` | 质疑假设、跨课题传导、补强要求 | Round 3 |
| 交叉评审席 | A/B/C 互评 | 同行评议、打分、投票 | Round 4 |

## 流程概览

```
Round 0  准备 + 假设框定（CIO）
  │
  ├──→ Round 1  三研究员独立调研（并行）
  │
  ├──→ Round 2  魔鬼辩护人构建反方（与 Round 1 并行）
  │
Round 3  基金经理审阅 + 跨课题传导（PM）
  │
Round 4  深度研究 + 交叉评审（多轮收敛）
  │         ↱ 分歧未收敛 → 补一轮
Round 5  投资总监综合（CIO）
  │
Round 6  写入仓库 + 增量追踪（CIO）
```

## 课题优先级

| 批次 | 课题 | 理由 |
|------|------|------|
| Batch 1 | #07, #08, #17 | 最高评级 + 催化剂密集 |
| Batch 2 | #04, #11, #21 | 有条件通过↑ 或 通过↑，能见度高 |
| Batch 3 | #01, #06 | 技术关注，需判断是否升级 |
| Batch 4 | 其余 12 个 | 按优先级轮转 |

## 输出位置

分析结果存入对应课题的 `updates/` 目录：
```
mega-trends/07_xxx/updates/
  YYYY.MM.DD_round_N/
    _synthesis.md                 ← 唯一必读文件
    researcher_A_fundamental.md
    researcher_B_catalyst.md
    researcher_C_macro.md
    devil_advocate.md
    pm_review.md
    peer_reviews.md
```
