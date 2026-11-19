---
name: pezim-swing-scan
description: |
  按 Brian Pezim《How to Swing Trade》做股票收盘扫描，比较市场宽度与板块强弱，整理常规形态、隔夜动量及热门板块候选，生成带次日触发、失效和待核事项的观察清单。
metadata:
  cangjie.generated-by: cangjie-tools v2.5.0
  cangjie.variant: single
  cangjie.bundle-id: bundle.pezim
  cangjie.capability-count: 8
  cangjie.entrypoint-count: 1
---
# How to Swing Trade — 全书能力入口

## 触发与不触发

**适用**：与本书能力域相关的咨询与任务（见下方路由表的意图列）。
**不适用**：
- 自动下单、保证收益、长期内在价值估算。

## 核心原则（常驻速览，概览类问题读到这里即可回答）

1. 完整收盘扫描从 routine 卡和 resources/watchlist.md 开始，按本次重点补读一张策略卡。单项请求按路由表直接读取对应卡。
2. 确认交易日、交易所时区、股票池与截止时间。优先用用户给定的筛选导出或图表。请求当日市场且未给数据时，用可用行情与公告源获取并列明来源、时间、覆盖与延迟。历史重演只使用当时已知的资料。
3. 交付市场与板块摘要、逐股观察表和排除理由。每行含方向、策略证据、次日触发、拟价/止损/目标、收益÷风险、事件和状态。同一标的合并，缺项列待核。
4. 区分观察、条件触发与实际成交。仅有收盘快照的隔夜标的只能复盘信号或安排次日观察。盘前若跳价，按新拟价重算。

## 能力路由（先读本表，按意图加载 1 张能力卡）

| 用户意图 | 先读 | 补读/备注 |
|---|---|---|
| 解释市场参与度及行业周月强弱，判断方向是否一致 | references/capabilities/market.md | references/capabilities/screen.md、references/capabilities/gap.md |
| 从股票池筛出趋势延续或反转候选并记录过滤条件 | references/capabilities/screen.md | references/capabilities/chart.md、references/capabilities/events.md |
| 检查消息首日、尾盘延续与不利跳空情景 | references/capabilities/gap.md | references/capabilities/risk.md、references/capabilities/events.md |
| 区分题材的早期证据、跟风股与过热迹象 | references/capabilities/mania.md | references/capabilities/chart.md、references/capabilities/events.md |
| 为形态标出触发、失效与最近目标 | references/capabilities/chart.md | references/capabilities/risk.md、references/capabilities/screen.md |
| 辨别已公布消息与待公布二元事件、流动性及财务风险 | references/capabilities/events.md | references/capabilities/risk.md、references/capabilities/gap.md |
| 复算做多做空的收益风险、风险预算和拟议仓位 | references/capabilities/risk.md | references/capabilities/chart.md、references/capabilities/routine.md |
| 收盘生成次日计划，复核入场漂移、分批退出和执行偏差 | references/capabilities/routine.md | references/capabilities/risk.md、references/capabilities/market.md |

**非能力类查询**：
- 书名/作者/章节/整书概览 → references/overview.md
- 术语解释 → references/glossary.md
- 决策规则速查（不需要原文依据时） → references/cheatsheet.md
- 完整意图与关键词索引（本表未覆盖的意图先查这里） → references/capability-index.md

## 加载规则

- 每次任务先读本文件，再按路由表加载 **1** 张能力卡；任务明确跨域时最多加载 2 张。
- 概览/书名类问题不加载能力卡，用「核心原则」与 overview.md 回答。
- 路由表与 capability-index.md 都无法命中的意图，明确告知超出本书范围，不要硬套。

## 边界与判停

- 无法获得行情时交付可执行的筛选参数和待补字段，不编造标的、事件、实时价或全市场排名。
