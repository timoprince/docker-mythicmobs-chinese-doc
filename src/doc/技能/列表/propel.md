技能: Propel (4.14)
--------------------------

朝技能目标冲刺（不提供上下速度）  
拥有惯性 

修改项
----------

| 修改项名 | 别称    | 描述                                                                                                    | 默认值 |
|-----------|------------|----------------------------------------------------------------------------------------------------------------|---------------|
| velocity  | v, magnitude       | 冲刺速度 | 1             |

示例
--------

```yaml
    Skills:
    - propel{velocity=5} @forward{f=1}
```
令施法者以"5"的速度朝视野正前方1格冲刺

额外信息
-------

- **支持** [占位符](/技能/占位符)（仅限值类型为数值的修改项）