# 强化学习实验记录
观察后调整reward
修复collision没置上的错误

## 1. 实验基本信息

| 字段 | 内容 |
|---|---|
| 实验编号 | yyh-pvp-campclose-01051624x |
| 实验名称 | PVP campclose |
| 实验日期 | 2026-01-05 |
| 负责人 | Yuhan Ye |
| 项目 | G |
| Commit | default |
| 实验状态 | 进行中 |

## 2. 实验目标

| 项目 | 描述 |
|---|---|
| 1 | 初始化站位是否能带来团队决策的提升 |
| 2 | 身后射线特征和奖励能否减少撞墙 |
| 3 | JUMP CROUCH cd限制能否减少无意义蹲跳 |
| 对比方案 | baseline |

## 3. 环境与任务

| 项目 | 配置 |
|---|---|
| 地图 | 204/401 |
| Agent 数 | 3x4 |

## 4. Reward 设计
新增collision，观察是否减少向后撞墙
| Reward 项 | 数值
|---|---|
| is_win | 15 |
| kill | 5.0 |
| damage | 0.01 |
| shield_parry | 1 |
| shield_parry2 | 2 |
| crystal_parry | 2 |
| rapier_parry | 2 |
| take_damage | 0.01 |
| dead | 10.0 |
| jump_crouch | 0.02 |
| last_move_succeed | 0.00 |
| potion_hit | 2 |
| elude_failed | 0.01 |
| collision | 0.01 |


## 5. 实验变量

damage epoch < 50 *1.25
takeDamage epoch < 50 *0.75

## 6. 结果


## 7. 问题与结论


