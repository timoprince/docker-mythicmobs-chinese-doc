技能: Shoot Fire Ball
--------------------------

向技能目标发射火球.

修改项
----------

| 修改项名 | 别称    | 描述                                                                                                    | 默认值 |
|-----------|------------|----------------------------------------------------------------------------------------------------------------|---------------|
| yield         | y         | 火球爆炸威力                                 | 1             |
| velocity      | v         | 火球飞行速度                                 | 1             |
| incendiary    | i         | 是否形成火焰                      | false         |
| fireTicks     | ft        | 所形成的火焰持续时间             | 0             |
| smallfireball | small,sml | 是否为小火球而不是恶魂火球 | false         |
| playsound     | ps        | 是否在发射时播放音效  | false         |
| type          |           | 火球类型.SMALL(小)/LARGE(大)/DRAGON(末影龙弹) | SMALL |

修改项: type 新增于 MM 4.11

示例
--------

```yaml
发射火球示例:
 Skills:
 - shootfireball{y=1;v=4} @target
```
向仇恨目标发射飞行速度为`4`, 爆炸威力为1 的火球