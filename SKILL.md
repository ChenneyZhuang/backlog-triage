---
name: backlog-triage
description: |
  Triage a scattered backlog into a bounded queue of decisions: sweep every
  source (notes, chat pins, inbox flags, stale lists) into one inventory,
  classify each item into six dispositions — now / next / scheduled / waiting /
  reference / drop — with a stated reason, batch the commitment-changing
  items into one approval set for the user, and write the list back dated
  with drops archived by reason. Use when the user asks to sort out their
  todos, clean up a task list, plan the week or day, decide what to work on
  next, or when a backlog has grown unbounded and nothing in it is trusted.
  触发词：待办整理 / 任务分诊 / 清单清理 / backlog。
license: MIT
metadata:
  version: "0.1.0"
---

# Backlog Triage: a list that only grows is not a plan

Turn a backlog into a bounded queue of decisions. Items that were silently
abandoned resurface as guilt; "urgent" defaults to whoever asked last.
Dispositions with reasons fix both.

## Rules

1. **Sweep every source before classifying anything.** The inventory comes
   from all the places items hide — notes, chat pins, inbox flags, the
   previous list. A triage over one source re-buries the rest.
2. **Every item gets exactly one disposition and one reason.**
   - now — this session, before anything new starts
   - next — first pick when capacity frees up
   - scheduled — carries a real date; a dateless "later" is a drop
   - waiting — names the person who owes the next move and the ask
   - reference — information, not a task; it moves out of the queue
   - drop — leaves the list; the reason is recorded, not erased
3. **Drop is a decision, not an accident.** Dropped items land in an
   archive section with the reason, so abandoning is visible and
   reversible in one step.
4. **Commitments change through the user.** Any disposition that moves a
   deadline, cuts scope, or cancels a promise to another person goes into
   one approval batch; the agent drafts, the user sends.
5. **The triage output is small.** A useful session queue holds a handful
   of `now` items; a triage that returns thirty urgent things triaged
   nothing.

## Steps

1. **Inventory.** Sweep all sources into one undifferentiated list, counts
   per source stated. Done when: no known source is uncited and duplicates
   are merged.
2. **Classify.** Apply the six dispositions with a reason per item.
   Done when: every item carries exactly one disposition and one reason.
3. **Batch the commitments.** Collect every item that changes a promise to
   someone else into one approval set with the proposed message per item.
   Done when: the user receives one batch, not a stream of pings.
4. **Write back.** Produce the triaged list: dated, dispositions visible,
   drops archived with reasons, waiting items showing their pending ask.
   Done when: the list stands alone — a reader needs no chat history to
   trust it.

## Done when

Every item from every source carries a disposition with a reason, drops are
archived rather than vanished, commitment changes sit in one approval batch,
and the resulting queue is small enough to be a plan instead of a wall.
