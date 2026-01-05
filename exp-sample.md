# 强化学习实验记录

## 1. 实验基本信息

| 字段 | 内容 |
|---|---|
| 实验编号 | RL-2026-01-05-Exp03 |
| 实验名称 | 加入 entity max pooling 的 PVPVE 稳定性测试 |
| 实验日期 | 2026-01-05 |
| 负责人 | Yuhan Ye |
| 项目 | PVPVE Dungeon |
| 代码分支 | rl/maxpool_v2 |
| Commit | a3f92c1 |
| 实验状态 | 进行中 |

## 2. 实验目标

| 项目 | 描述 |
|---|---|
| 核心问题 | max pooling 是否提升稳定性 |
| 对比方案 | baseline / max pool / max pool + attention |

## 3. 环境与任务

| 项目 | 配置 |
|---|---|
| 地图 | map_dungeon_03 |
| Agent 数 | 4v4 + monsters |
| 观测频率 | 30 Hz |
| 动作空间 | 移动 / 转向(-8~8) / 射击 / 技能 |

## 4. Reward 设计

| Reward 项 | 数值 | 说明 |
|---|---|---|
| 击杀 | +1.0 | 最终击杀 |
| 命中 | +0.05 | 每次命中 |
| 靠近掩体 | +0.01 / m | 引导走位 |
| 被命中 | -0.1 | 受伤 |

## 5. 训练配置

| 参数 | 数值 |
|---|---|
| Total Steps | 50M |
| Batch Size | 8192 |
| Learning Rate | 3e-4 |

## 6. 实验变量

| 实验组 | 网络 | Reward |
|---|---|---|
| A | baseline | 原始 |
| B | max pool | 原始 |
| C | max pool + attn | 原始 |

## 7. 结果

| 指标 | 数值 |
|---|---|
| Mean Reward | 0.92 |
| Win Rate | 63% |

## 8. 问题与结论

| 项目 | 内容 |
|---|---|
| 问题 | attention 不稳定 |
| 结论 | max pool 更可靠 |
