技能: Remove Tag
--------------------------

移除技能目标身上的指定标签.

修改项
----------

| 修改项名 | 别称    | 描述                                                                                                    | 默认值 |
|-----------|------------|----------------------------------------------------------------------------------------------------------------|---------------|
| tag | t | 被移除标签的名称 | defaut |

示例
--------

```yaml
 Skills:
 - removetag{t=测试} @self
```
移除自身身上的标签: 测试