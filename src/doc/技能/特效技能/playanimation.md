特效技能: Play Animation
--------------

令技能目标播放指定原版动作

---

修改项
---

| 修改项名 | 别称    | 描述                                                                                                    | 默认值 |
|-----------|------------|----------------------------------------------------------------------------------------------------------------|---------------|
| animation           | a.effect,e     | 所播放的动作代数 | 1              |

新增于 MM 4.14.0

动作代数
---

| 代数 | 描述 |
| - | - |
| 0 | 正常 |
| 1 | 受伤 |
| 2 | 死亡 |

---



示例（实体配置）
---

```
 Skills:
 - playanimation{a=0} @self ~onAttack
```

额外信息
---

- **支持** Audience
- **支持** [占位符](/技能/占位符)
- 别称: effect:playanimation e:playanimation