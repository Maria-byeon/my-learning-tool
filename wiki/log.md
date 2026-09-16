---
type: log
created: 2026-09-09
---

# 操作日志

> 按时间倒序记录本知识库的所有写入、重组、链接变更。
> 每条记录尽量给出日期、时间、动作、相关路径，便于回溯。

## 2026-09-09

### 11:34 — 初始化 wiki 体系骨架

- 新增目录：`raw/`、`raw/papers/`、`wiki/`、`wiki/sources/`、`wiki/entities/`、`wiki/concepts/`、`wiki/syntheses/`
- 新增文件：
  - `wiki/index.md` — 知识库入口与目录索引
  - `wiki/log.md` — 本文件
  - `wiki/overview.md` — 全局知识综述（占位）
  - `raw/.gitkeep`、`raw/papers/.gitkeep`、`wiki/sources/.gitkeep`、`wiki/entities/.gitkeep`、`wiki/concepts/.gitkeep`、`wiki/syntheses/.gitkeep` — 目录占位与用途说明
- 约定：
  - `raw/` 内容**只读**，观点写入 `wiki/`
  - 子页面统一使用 frontmatter（`type` / `tags` / `created` / `status`）
  - 双向链接使用 `[[page-name]]` 形式

## 2026-09-16

### 11:45 — 首次 ingest：小红书 · 柚柚豆王

- 摄入文件：`wiki/sources/小红书-柚柚豆王.md`
- 摄入来源：`https://xhslink.cn/o/ADjYqbNmAEp`（小红书短链，302 到 `xiaohongshu.com/user/profile/5eb7cbd10000000001003a9d`）
- 抓取方式：CDP 直连（Edge `--remote-debugging-port=9222` + Node 脚本 `Runtime.evaluate` 抓 DOM），绕过 Kimi 扩展（扩展链路 `extension_connected:false` 仍未通）
- 抓取脚本：`~/.kimi-webbridge/cdp_xhs.js`（首轮）、`~/.kimi-webbridge/cdp_xhs_detail.js`（二轮）
- 截图：`~/.workbuddy/memory/xhs-account.png`
- 关键内容：
  - 账号画像：22 岁 / 甘肃 / 小红书号 468372250 / 免费拼豆图纸日更
  - 数字：关注 10+ / 粉丝 10+ / 获赞与收藏 1千+
  - 24 篇作品全拼豆主题，TOP3 均蜡笔小新系（397 / 100 / 84）
- 双向链接占位：[[拼豆]] / [[小红书账号运营]] / [[小红书数据脱敏口径]] / [[蜡笔小新]] / [[Hello Kitty]]（均待建）
- 同步更新：`wiki/index.md`「当前条目」段加入该条目