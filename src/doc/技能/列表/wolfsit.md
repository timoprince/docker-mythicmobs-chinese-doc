技能: Wolf Sit　(4.11)
--------------------------

令技能目标（狗）站起或坐下.

修改项
----------

| 修改项名 | 别称    | 描述                                                                                                    | 默认值 |
|-----------|------------|----------------------------------------------------------------------------------------------------------------|---------------|
| state | 无 | 是否坐下, 为否时站起 | 无 |

示例
--------

```yaml
 Skills:
 - wolfsit{state=false} @self
```
令自身(实体种类为狗)站起.