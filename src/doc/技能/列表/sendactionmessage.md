技能: Send Action Message
--------------------------

向技能目标（玩家）发送活动栏信息.

修改项
----------

| 修改项名 | 别称    | 描述                                                                                                    | 默认值 |
|-----------|------------|----------------------------------------------------------------------------------------------------------------|---------------|
| message   | m       | 用于发送的信息,用""包裹 | 无 |

示例
--------

```yaml
 Skills:
 - actionmessage{m="<mob.name>&f 释放了技能!"} @PlayersInRadius{r=30}
```
向半径30格方块范围内的所有玩家发送活动栏消息: `(施法者名) 释放了技能!`

额外信息
---

- [x] 别称: actionmessage, am