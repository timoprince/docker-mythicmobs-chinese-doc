特效技能: Particle Ring
--------------------------

于目标位置生成由粒子组成的空心环.

修改项
----------

| 修改项名 | 别称    | 描述                                                                                                    | 默认值 |
|-----------|------------|----------------------------------------------------------------------------------------------------------------|---------------|
| amount | a | 环上每个点所使用的粒子数量 | 1 |
| points | p | 环由多少个点组成 | 10 |
| radius          | r        | 环半径(格方块) | 10            |
| yoffset | y | 环中心的垂直偏移量(格方块) | 0 |

示例
--------

```yaml
 Skills:
 - effect:particlering{particle=flame;radius=20;points=32;amount=1;hS=1;vS=0} @target
```

额外信息
---

- 别称: e:particlering, particlering, e:pr, pr
