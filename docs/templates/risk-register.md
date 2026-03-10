# Risk Register Template

## Purpose
Maintain a living list of project risks so the team can proactively mitigate issues before they become blockers. Store this file in `docs/` and update it at every weekly sync. Reference it from the project README or Project Charter.

## How to use
1. Add a row for each identified risk.
2. Review and update the **Status** column at every weekly delivery sync.
3. Link high-impact risks to GitHub Issues so they appear on the project board.
4. Archive resolved risks by setting Status = Closed and moving the row to the **Closed Risks** section.

---

## Active Risks

| ID | Description | Impact | Likelihood | Score* | Owner | Mitigation Plan | Status | Last Updated |
|---|---|---|---|---|---|---|---|---|
| RISK-001 | _Example: Third-party API may hit rate limits under load_ | High | Med | 6 | @owner | Implement client-side retry and exponential back-off | Open | YYYY-MM-DD |
| RISK-002 | | | | | | | | |

> **Score** = Impact × Likelihood using: High=3, Med=2, Low=1. Score ≥ 6 = critical; 3–5 = moderate; 1–2 = low.

---

## Closed Risks

| ID | Description | Resolution | Closed Date |
|---|---|---|---|
| | | | |

---

## Risk Review Log

| Date | Reviewer | Changes Made |
|---|---|---|
| YYYY-MM-DD | @pm | Added RISK-001 |

