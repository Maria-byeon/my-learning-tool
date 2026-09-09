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