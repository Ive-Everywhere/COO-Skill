---
name: gtm-watchtower
description: Analyzes GTM (Go-to-Market) data to flag risks in Pipeline, Commit, and Churn.
---

# GTM WATCHTOWER LOGIC

## 1. Flexible Trigger Protocols
Respond to specific commands OR natural language queries (e.g., "How is the APAC pipeline?").

## 2. Analysis Protocols

### [cite_start]IF HUNTING POD (APAC, EMEA, AMER 1-3, Corp, GSI)[cite: 18]:
Check for these specific Red Flags:
1.  [cite_start]**Variance:** Has Forecast Commit changed >10% vs last week? [cite: 21]
2.  [cite_start]**Stalled ("Ghost Deal"):** Is the deal in "Commit" stage with NO activity >14 days? [cite: 22]
3.  [cite_start]**Coverage:** Has pipeline coverage dropped below 3x target? [cite: 24]

### [cite_start]IF FARMING POD (AM Teams)[cite: 25]:
Check for these specific Red Flags:
1.  [cite_start]**Churn Risk:** Renewal Date <90 days AND Health Score = Red/Yellow[cite: 29].
2.  [cite_start]**Expansion:** License utilization >85% (Flag as Upsell Opportunity)[cite: 30].

## 3. Output Routing
* **GTM Risks:** Format as an alert for `#supernautprime-gtm-radar`.
* [cite_start]**Format:** Use "The Firm Coach" archetype (Observation -> Inquiry -> Remediation)[cite: 76].
