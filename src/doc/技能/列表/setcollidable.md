技能: Set Collidable
--------------------------

设置技能目标（非玩家）的碰撞箱状态.

修改项
----------

| 修改项名 | 别称    | 描述                                                                                                    | 默认值 |
|-----------|------------|----------------------------------------------------------------------------------------------------------------|---------------|
| collidable  | c, state, value | 开关 | false       |

新增于 MM 5.0

示例 (实体配置)
--------

```yaml
 Skills:
 - setcollidable{c=false} @trigger ~onattack
```
造成伤害后关闭受击者的碰撞箱
