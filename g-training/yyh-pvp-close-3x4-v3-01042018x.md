# 强化学习实验记录

## 1. 实验基本信息

| 字段 | 内容 |
|---|---|
| 实验编号 | yyh-pvp-close-3x4-v3-01042018x |
| 实验名称 | PVP close 3x4 |
| 实验日期 | 2026-01-04 |
| 负责人 | Yuhan Ye |
| 项目 | G |
| Commit | default |
| 实验状态 | 结束 |

## 2. 实验目标

| 项目 | 描述 |
|---|---|
| 1 | 初始化站位能否加快训练 |
| 2 | 减少训练AI个数能否降低action fail rate |
| 3 | 课程学习damage/take damage是否更合理 |
| 对比方案 | baseline |

## 3. 环境与任务

| 项目 | 配置 |
|---|---|
| 地图 | 204/401 |
| Agent 数 | 3x4 |

## 4. Reward 设计
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
| dead | 5.0 |
| jump_crouch | 0.02 |
| last_move_succeed | 0.00 |
| potion_hit | 2 |
| elude_failed | 0.01 |


## 5. 实验变量

-	初始化站位更加接近
-	3x8 -> 3x4
-	damage 50 EPOCH前 * 1.5， takeDamage 50EPOCH前 / 2


## 6. 结果
初始化站位能加速训练
3x4能降低动作失败率，但仍有30+
课程学习更加合理，避免前期学习失败，后期能收敛

## 7. 问题与结论


