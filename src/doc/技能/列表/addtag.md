技能: Add Tag
--------------------------

为技能目标添上指定名称的标签.

修改项
----------

| 修改项名 | 别称    | 描述                                                                                                    | 默认值 |
|-----------|------------|----------------------------------------------------------------------------------------------------------------|---------------|
| tag | t | 所添加标签的名称 | defaut |

示例
--------

```yaml
 Skills:
 - addtag{t=测试} @self
```
为自身添上标签: `测试`