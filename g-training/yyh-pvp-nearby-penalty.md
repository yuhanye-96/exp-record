# 强化学习实验记录


## 1. 实验基本信息

| 字段 | 内容 |
|---|---|
| 实验编号 | yyh-pvp-nearby-penalty-01062042x |
| 实验名称 | PVP add nearby penalty |
| 实验日期 | 2026-01-06 |
| 负责人 | Yuhan Ye |
| 项目 | G |
| Commit | default |
| 实验状态 | 进行中 |

## 2. 实验目标

| 项目 | 描述 |
|---|---|
| 1 | 近处damage减少，远程增加， 观察弓箭手和牧师是否还贴脸攻击，是否还喜欢跳攻击 |
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

< 2m  damage * 0.2
> 2m  damage * 1.2

## 6. 结果


## 7. 问题与结论


