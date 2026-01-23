# 强化学习实验记录


## 1. 实验基本信息

| 字段 | 内容 |
|---|---|
| 实验编号 | yyh-pvp-teamcenter-01202036x |
| 实验名称 | PVP add team center |
| 实验日期 | 2026-01-22 |
| 负责人 | Yuhan Ye |
| 项目 | G |
| Commit | default |
| 实验状态 | 进行中 |

## 2. 实验目标

| 项目 | 描述 |
|---|---|
| 1 | 增加队伍中心概念 |
| 对比方案 | baseline |

## 3. 环境与任务

| 项目 | 配置 |
|---|---|
| 地图 | 204/401 |
| Agent 数 |80% 3x4 、20% 1x12|

## 4. Reward 设计
| Reward 项 | 数值
|---|---|
| is_win | 15 |
| kill | 5.0 |
| warrior_damage | 0.01 |
| ranger_damage | 0.01 |
| priest_damage | 0.01 |
| warrior_take_damage | 0.01 |
| ranger_take_damage | 0.01 |
| priest_take_damage | 0.01 |
| shield_parry | 1 |
| shield_parry2 | 2 |
| crystal_parry | 2 |
| rapier_parry | 2 |
| dead | 10.0 |
| jump_crouch | 0.02 |
| last_move_succeed | 0.00 |
| potion_hit | 2 |
| elude_failed | 0.01 |
| collision | 0.02 |
| heal | 0.05 |

## 5. 实验变量
feature num：2314

## 6. 结果

## 7. 问题与结论



