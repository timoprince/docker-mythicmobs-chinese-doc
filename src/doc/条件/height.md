**描述:** 若实体所处位置的Y轴坐标在指定范围内.

修改项
---

| 修改项名  | 别称           | 描述                      |
| --------- | -------------- | ------------------------- |
| height | h | 用于检测的Y轴坐标数值范围 |

示例
---

```yaml
 Conditions:
 - height{h=<50} true
```

拓展信息
---

- 检测对象: 位置