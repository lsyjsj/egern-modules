# egern-modules

自用 Egern 模块合集。每个模块独立放在一个目录下，目录名即模块名。

## 模块列表

| 目录 | 模块 | 说明 |
| --- | --- | --- |
| `unicom/` | 中国联通小组件（三号码独立版） | 3 个手机号各显示为一个独立小组件：话费 / 语音 / 流量（含定时保活）。改自 [IBL3ND/module](https://github.com/IBL3ND/module) 的 `CT_Widget.yaml`，抓包与缓存按号码隔离 |

## Egern 订阅方式

Egern → 工具 → 模块 → 右上角 ＋ → 粘贴对应目录下 `.yaml` 文件的 raw 链接，例如：

```
https://raw.githubusercontent.com/lsyjsj/egern-modules/main/unicom/CT_Widget_3num.yaml
```

## unicom 模块使用说明

1. 在模块 Env 页填写 `CU_PHONE_1/2/3`（要显示的 3 个联通手机号）。
2. 分别用联通 App 登录每个号码并打开一次，脚本会自动抓取各号码的登录信息（按号码分别存储，互不覆盖）。
3. 回桌面添加 Egern 小组件，编辑时选择「中国联通·号码1/2/3」。
