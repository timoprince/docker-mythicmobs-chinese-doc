特效技能: Ender Beam
--------------------------

创建末影水晶以朝指定位置发射光束.

修改项
----------

| 修改项名 | 别称    | 描述                                                                                                    | 默认值 |
|-----------|------------|----------------------------------------------------------------------------------------------------------------|---------------|
| duration  | d      | 光束持续时间(刻)  | 60            |
| yoffset   | y, yo  | 	光束发射点垂直偏移量(格方块) | 0             |

示例
--------

```yaml
 Skills:
 - effect:enderbeam{d=100;y=2} @target
```

额外信息
---

- 别称: enderbeam