技能: Set Max Health
--------------------------

设置技能目标的最大生命.

修改项
----------

| 修改项名 | 别称    | 描述                                                                                                    | 默认值 |
|-----------|------------|----------------------------------------------------------------------------------------------------------------|---------------|
| amount | a | 修改后的最大生命（支持[占位符](/占位符)） | 1.0 |
| mode | m | 设置模式,STATIC为直接设置最大生命值,SCALE在其基础上会恢复等值于 新最大生命比原最大生命多的百分比 的生命值 | STATIC |

示例（实体配置）
--------

被右键后设置自身最大生命为5
```yaml
 Skills:
 - setmaxhealth{amount=5;mode=STATIC} @self ~onInteract
 - ...
```
被右键后设置自身最大生命为5并恢复生命
```yaml
 Skills:
 - setmaxhealth{amount=5;mode=SCALE} @self ~onInteract
 - ...
```