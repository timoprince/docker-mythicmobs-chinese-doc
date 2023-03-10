技能: On Damaged (4.8)
--------------------------

给予技能目标[光环](技能/列表/Aura)(光环持有者受到任何形式的伤害后激活技能组).  
该光环被锁定在主线程进行（即使Sync已为false）  
光环触发者为攻击自身的实体

可使用技能: [Aura](/技能/列表/aura) 的全部修改项（如onstartskill）

修改项
----------

| 修改项名 | 别称    | 描述                                                                                                    | 默认值 |
|-----------|------------|----------------------------------------------------------------------------------------------------------------|---------------|
| ondamagedskill | ondamaged, od, onhitskill, onhit, oh | 光环持有者受到伤害后所激活的技能（光环给予者为技能施法者） | 无 |
| cancleevent | cancel, cE, canceldamage, cd | 光环持有者受到伤害后是否取消受到伤害事件 | false |
| damageSubtract | sub, s | 光环持有者所受到伤害的数值所被减去的具体数值（4.11起支持[占位符](/技能/占位符)） | 0 |
| damageMultiplier | multiplier, m | 光环持有者所受到伤害的数值所被乘以的百分比（4.11起支持[占位符](/技能/占位符)） | 1 |
| damageModifiers | damageMods | 伤害数值计算后<br>根据该修改项的值对其进行二次调整<br>工作方式类似于[伤害调整](/实体/伤害调整)<br>多个之间用","隔开 | 无 |

详细信息
-------

- 可被任意形式的伤害所激活（包括窒息、燃烧）
- **无法** 无视受伤间隔, 但取消事件将直接清空受伤间隔
- **可以** 被该技能组所激活的技能激活（如 [Damage](/技能/列表/damage) ）
- 可被自身所激活的技能激活（不由光环激活此技能）
- 调整值为负数, 施法者将额外扣血
- 调整后的值为负数, 施法者将 **永远** 不会受到伤害, 且生命值越打越多（不会超过最大生命）
- <skill.var.damage-amount>变量 显示的是 调整前的伤害数值 而不是调整后
- **CancelOnTakenDamage** 为 true 时, 若该光环的 `cancelevent` 为true, 则不会被正常执行

子技能组相关
---

- 若MM版本<5.0, onHitSkill的默认技能目标将会是拥有该光环的实体  
- 若MM版本≥5.0, onHitSkill的默认技能目标将会是造成伤害的实体（对于onDamaged而言） 
如: `- onattack{oh=[  - m{m=1} ];d=999} @self`  
在MM 4.11 将会把消息发送给施法者  
在MM 5.2.0 却会发送给对光环持有者造成伤害的实体


示例
--------

       Skills:
      - onDamaged{oH=受伤释放;cancel=true;auraname=受伤光环;d=100}

5秒内无敌

       Skills:
      - onDamaged{oH=受伤释放;cancel=true;auraname=受伤光环;m="Fire 0.5,Projectile 0,测试 2";d=200}

10秒内免疫弹射物伤害, 灼烧伤害减半, 额外受到一倍伤害类型为"测试"的伤害