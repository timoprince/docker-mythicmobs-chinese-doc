技能: Set Raider Patrol Block
--------------------------

令施法者（掠夺者）向技能目标所处位置巡逻

修改项
----------

| 修改项名 | 别称    | 描述                                                                                                    | 默认值 |
|-----------|------------|----------------------------------------------------------------------------------------------------------------|---------------|
| location | l | b | 巡逻中心位置的三轴坐标, 值格式为: `x,y,z` | |

示例
--------

```yaml
 Skills:
 - setRaiderBlock @nearestplayer{r=100} ~onTimer:200
 - ...
```
施法者每10秒向距自身距离不到100的玩家的所处位置巡逻

拓展信息
-------

- 别称: setRaiderBlock