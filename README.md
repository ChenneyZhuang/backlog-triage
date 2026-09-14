# backlog-triage 待办分诊

A backlog that only grows is not a plan — it is an anxiety list. Turn it into a bounded queue of decisions.

只进不出的待办清单不是计划，是焦虑清单。把它变成一组有限的决策。

## Why / 为什么

Backlogs fail in two directions: items that were silently abandoned keep resurfacing as guilt, and "urgent" is whoever asked last. The fix is dispositions with reasons — every item leaves the triage with exactly one of six fates, and dropping is an explicit decision rather than an accident.

待办清单的两种失败：被默默放弃的事项反复浮现成负罪感；"紧急"等于谁最后催了谁。解法是带理由的分类——每条待办分诊后恰好落到六种命运之一，放弃是显式决策而非意外。

## The six dispositions / 六种分类

| Disposition | Meaning |
|---|---|
| now | this session, before anything new |
| next | first pick when capacity frees up |
| scheduled | dated and parked — the date is visible |
| waiting | someone else owes the move; the ask is named |
| reference | information, not a task |
| drop | leaves the list; the reason is recorded |

## How it runs / 怎么跑

1. **Sweep** every source — notes, chat pins, inbox flags, the previous list — into one inventory.
2. **Classify** each item with a reason; cluster the `now` set so the session has at most a handful.
3. **Reconcile commitments** — anything that changes a promise to another person (deadline moves, scope cuts) goes into one approval batch for the user; the agent drafts, the user sends.
4. **Write the list back** — dated, dispositions visible, dropped items recorded with their reason in an archive section instead of deleted silently.

Rules that do the work: *scheduled means a real date or it is not scheduled*; *waiting means the pending move is named*; *drop is a decision, so it gets a reason and an archive line*.

## Honest limitations / 如实说明局限

- Triage quality is bounded by the honesty of the drop reasons; "drop" with a fake reason is procrastination in costume.
- Commitment changes still need the user's real approval — the skill drafts, humans decide.

分诊质量取决于放弃理由的诚实度；假理由的"放弃"是穿着马甲的拖延。承诺变更仍需用户真实批准——skill 起草，人拍板。

## Install / 安装

```bash
npx skills add ChenneyZhuang/backlog-triage
```

Per-agent paths and runtime requirements: see [COMPATIBILITY.md](COMPATIBILITY.md). MIT. v0.1.0.

各 agent 安装路径与运行时要求见 COMPATIBILITY.md。MIT 许可，v0.1.0。
