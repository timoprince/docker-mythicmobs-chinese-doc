技能: Leap
--------------------------

向技能目标冲刺  
冲刺附着惯性

修改项
----------

| 修改项名 | 别称    | 描述                                                                                                    | 默认值 |
|-----------|------------|----------------------------------------------------------------------------------------------------------------|---------------|
| velocity | v | 冲刺速度 | 100 |
| noise | n | 偏移程度 | 1 |

示例
--------

```yaml
冲刺技能测试:
 Cooldown: 10
 Skills:
 - leap{velocity=200} @target
 - delay 20
 - jump{velocity=-100}
 - effect:explosion @self
 - damage{amount=20} @EntitiesInRadius{r=5}
```

额外信息
--

- **支持** [占位符](/技能/占位符)