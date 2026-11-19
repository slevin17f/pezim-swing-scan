# pezim-swing-scan

用 Brian Pezim 在《How to Swing Trade》（2018）中介绍的方法，把股票收盘数据整理成次日观察清单。八张中文能力卡覆盖市场宽度、板块强弱、常规扫描、隔夜动量、热门题材、图表、事件与风险复核，以及次日跟踪。

## 安装

下载本仓库并解压，将 `skills/pezim-swing-scan` 整个目录复制到个人的 `~/.agents/skills/`，或项目的 `.agents/skills/`。在新的 Codex 会话中调用 `$pezim-swing-scan`。技能由 Markdown 文件组成，无需安装软件包。扫描用的行情、图表和事件日期由调用方提供或从可用数据源取得。

## 示例

> 用 $pezim-swing-scan 检查这份收盘筛选表。把已碰到前期阻力和即将发财报的股票单列，写出其余候选明天要满足的条件。若开盘跳价，按原止损和目标重新计算收益风险比。

[Skill 入口](skills/pezim-swing-scan/SKILL.md) · [收盘工作表](skills/pezim-swing-scan/resources/watchlist.md) · [能力索引](skills/pezim-swing-scan/references/capability-index.md)

## 方法来源

Brian Pezim, *How to Swing Trade: A Beginner’s Guide to Trading Tools, Money Management, Rules, Strategies and Routines of a Swing Trader*（2018）。本项目使用仓颉整理为中文工作流程。各卡给出原书章节和页码，工作表中的虚构数据标记为模拟示例。
