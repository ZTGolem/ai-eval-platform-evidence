# M5-10：统一前后端费用单位为 CNY

同一演示场景在改动前后截取的页面证据。

- 改动前：`origin/main` @ `3380527`，费用字段与展示为 USD。
- 改动后：`agent/unify-cny-billing-bfe28fc77f89` @ `66ec665`，费用字段与展示为 CNY。
- 场景：一个阿里云竞价池（当前价 0.10 USD/h ↔ 0.72 CNY/h，阈值 0.50 ↔ 3.60）、一个模型配置（输入 0.14 ↔ 1.008 CNY/百万 token，输出 0.28 ↔ 2.016）、一个 6 用例评测（预算 0.50 ↔ 3.60，已花费 0.20 ↔ 1.44）。
- 采集：1440×1000、zh-CN、浅色主题，Playwright + Chrome 截取真实页面（本地 API + Vite，演示数据等价）。
- 文件：`resources-list`、`resources-detail`、`resources-edit`、`models-list`、`models-detail`、`eval-detail` 的 `before-*` / `after-*` 成对截图。
