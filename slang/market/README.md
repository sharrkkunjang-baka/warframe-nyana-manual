# WM 市场物品别称（用户可编辑）

此目录只维护市场物品别称，不返回正文。

**路径注意**：
- ✅ 本目录 `source/slang/market/*.md`（`kind: market` → `marketAliases`）
- ✅ 顶层 `source/slang/market.md`（`## 英文规范名` + `别名：`）同样正式归类为 `market`，直接进入 `marketAliases`
- ✅ 顶层 `frames.md` / `mods.md` / `weapons.md` 等为正式 `domain` 别称，不再标记 legacy
- ❌ 不要改 `qq-bot/warframe-market-reviewed-aliases.md`；生产只读 content 权威源，改 MD 后执行 `wf重载 黑话`

热更新：
- 改本目录 `.md` 或顶层 `market.md` → `wf重载 黑话`（别名：`别名` / `slang`）
- 改 `source/command-prefix-filters.md` → 下一次 b/s/zk 请求按 mtime 自动生效，无需 `wf重载` 或重启
- 改 Runtime 市场解析 JS → `wf重载 市场`（别名：`wm` / `交易`）
无需整仓重启。市场查询读取当前 slang 快照里的 `marketAliases`，不会在每次 `wm` 时重新扫盘；短前缀过滤文件除外，它会按请求检查 mtime。

```markdown
# Primed Counterbalance
- 正式名：Primed Counterbalance
- 别称：制衡p、p制衡、制衡Prime
- 类型：mod

可选备注，不参与市场查询。
```

`正式名`可填写 WFM 英文正式名、官方简中、稳定 `gameRef/uniqueName` 或 WFM slug。绑定必须在当前 WFM 目录中唯一；不存在、歧义或类型不符时只隔离该条目。

兼容字段：`别称`/`别名`/`关键词`/`关键字`，兼容中英文冒号与顿号/逗号。常用类型：`mod`、`arcane`、`weapon`、`prime-part`、`set`、`lens`、`blueprint`、`component`。`riven-weapon` 保留给紫卡武器专用桥接，普通市场别称不会污染 ZK。

审核别称主文件：`reviewed-aliases.md`。也可按主题拆成多个 md。

解析优先级：WFM 英文正式名完整精确 ＞ 官方简中完整精确 ＞ 元素/派系核心黑话 ＞ 本目录审核别称完整精确 ＞ 原有统一解析器/拼音与受控模糊。别称不能覆盖正式名；冲突返回候选，不按最后写入覆盖。
