**描述:** 若最后一次收到的信号为.

修改项
---

| 修改项名  | 别称           | 描述                      |
| --------- | -------------- | ------------------------- |
| signal    | s     | 用于检测的信号名 |

示例
---

```yaml
 Conditions:
 - lastsignal{s=某信号} true
```

拓展信息
---

- 检测对象: 实体