技能: Modify Score
--------------------------

修改虚拟玩家指定记分板上的分数（上限2147483647）.  
虚拟目标名为玩家名, 相当于修改指定玩家的分数.

可用算法:

-   SET(设置)
-   ADD(加)
-   SUBTRACT(减)
-   MULTIPLY(乘以)
-   DIVIDE(除)
-   MOD(除以后取余)

修改项
----------

| 修改项名 | 别称    | 描述                                                                                                    | 默认值 |
|-----------|------------|----------------------------------------------------------------------------------------------------------------|---------------|
| objective | obj, o  | 用于修改的记分板名,不存在则创建 （支持[占位符](/技能/占位符)） |         |
| action    | a       | 算法                                                                                                         | ADD     |
| value     | v       | 修改值 （支持[占位符](/技能/占位符)） | 0 |  
| name | n, entry, e | 虚拟目标名 （支持[占位符](/技能/占位符)） | 无 |

示例
--------

```yaml
 Skills:
 - modifyscore{e=dummy;o=测试;v=1;a=SET} @self ~onInteract
```
右键后将dummy在记分板 测试 上的分数设为1