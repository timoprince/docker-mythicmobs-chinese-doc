特效技能: Particle Box
--------------------------

于技能目标位置生成一个不可见的方体, 随机选取方体内指定数量的点.

修改项
----------

| 修改项名 | 别称    | 描述                                                                                                    | 默认值 |
|-----------|------------|----------------------------------------------------------------------------------------------------------------|---------------|
| amount | a | 所选取的各点所显示的粒子数量 | 1 |
| radius    | r     | 正方体边长(格方块) | 5             |

示例
--------

```yaml
 Skills:
 - effect:particlebox{particle=flame;a=200;r=5} @self
```

额外信息
---

- 别称: e:particlebox, particlebox, e:pb, pb