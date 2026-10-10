# B2B 90-Day Lead Plan

[English](README.md) | [简体中文](README.zh-CN.md)

> Produce an executable 90-day lead-generation plan and an enquiry tracking ledger for a local B2B service business.

## What this is

> **Note on de-identification.** This README is written generically. The skill file itself may still reference internal domains, host names or local absolute paths. Run a scan pass (see `opensource-preflight-audit`) and replace them before publishing.

This is not a marketing strategy document. Strategy documents read well and change nothing.

The output here is a plan that has been forced down to the level of "which channel, which month, how many enquiries". If a line in the plan cannot be traced to an action someone can do next week, it does not belong in the plan.

## Why we open-sourced it

We build these for local service businesses, and the recurring problem was the same: an impressive plan that nobody executed because it described outcomes rather than actions.

The structure is generic. The demand allocation approach and the ledger format do not depend on the industry, so it is a reasonable thing to share.

## What it does

- **Demand allocated to channels and months.** The lead target is decomposed into per-channel, per-month quantities, rather than stated once and left there.
- **Each channel carries concrete actions** rather than a capability description.
- **A companion Excel ledger** for tracking enquiries, so the plan and the tracking live in the same system.
- **Two deliverables, one logic.** The Word plan and the Excel ledger describe the same structure and cannot drift apart.

## Requirements

None — methodology skill, no scripts

## Installation

```bash
git clone https://github.com/<your-username>/b2b-90day-lead-plan.git
```

Then place the folder into your agent skills directory:

| OS | Path |
|---|---|
| Windows | `C:\Users\<you>\.workbuddy\skills\b2b-90day-lead-plan\` |
| macOS / Linux | `~/.workbuddy/skills/b2b-90day-lead-plan/` |

There is no build step. Restart the session and it takes effect.

## How to use

State the business and the target:

- "I need a 90-day acquisition plan for <business>"
- "Three months, here's my enquiry target"
- "Which channels should I use, and how many leads each"

The skill asks for the business parameters first, then produces the plan and the ledger together.

## Files

```
└── SKILL.md
```

## Notes and limits

1. **The channel mix is a judgement, not a formula.** The skill structures the decision; it does not remove the need to make it.
2. **Capacity constrains the plan.** A target nobody can service is worse than an honest lower number.
3. **The ledger only works if it is used.** Tracking that stops in week three makes the plan unreadable by week six.
4. **References to specific businesses are examples** and should be replaced.

## License

MIT
