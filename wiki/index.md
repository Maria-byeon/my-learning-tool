---
type: index
created: 2026-09-09
status: active
---

# Wiki 目录

> 个人知识库的入口页。按内容类型分四个子目录；本页给出索引与导航约定。

## 主页面

- [[overview]] — 全局知识综述：跨主题的概念地图与核心脉络
- [[log]] — 操作日志：本知识库的写入、重组、链接变更记录

## 子目录

| 目录 | 用途 | 命名约定 |
|------|------|----------|
| `sources/` | 每份原始资料的摘要页 | `<slug>.md`，与 `raw/` 中原文件同名（去后缀） |
| `entities/` | 人物、公司、机构、产品、项目 | `<slug>.md`，单词小写或 `kebab-case` |
| `concepts/` | 想法、框架、模型、方法 | `<slug>.md`，英文/中文均可 |
| `syntheses/` | 跨条目的查询答案与综述 | `<YYYY-MM-DD>-<query-slug>.md` |

## 导航约定

- 双向链接使用 `[[page-name]]` 形式；通过 Obsidian / logseq 等工具解析。
- 每个页面顶部用 frontmatter 标注 `type`、`tags`、`created`、`status`。
- `raw/` 中文件**只读**，一切观点写入 `wiki/`。

## 当前条目

> 尚未摄入任何条目，等待首次 ingest。