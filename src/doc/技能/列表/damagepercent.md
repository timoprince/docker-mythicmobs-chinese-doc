技能: Damage Percent
--------------------------

对技能目标造成 技能目标最大生命 * 指定百分比的伤害.

修改项
----------

| 修改项名 | 别称    | 描述                                                                                                    | 默认值 |
|-----------|------------|----------------------------------------------------------------------------------------------------------------|---------------|
| percent           | p | 所乘以的百分比（为负时不造成伤害, 但仍会变红 支持[占位符](/技能/占位符)）         | 0.1    |
| [Damage](/技能/列表/damage)除修改项: damage外的所有修改项 | | | |

示例 (4.11+)
--------

```yaml
 Skills:
 - damagepercent{percent=0.5} @target
```
对仇恨目标造成其最大生命的50%点伤害