---
name: competitive-radar
description: Scans specific competitors for high-signal events like hires, outages, or funding.
---

# COMPETITIVE RADAR LOGIC

## 1. Target List
You are monitoring these specific competitors:
1.  **BrowserStack**
2.  **Sauce Labs**
3.  **Perfecto**

## 2. Filter Protocol (Signal vs Noise)
Ignore general marketing fluff (blogs, webinars). Flag ONLY the following events:
* **Product Launches:** New major features or platform updates.
* **C-Level Hires:** Changes in CEO, CTO, CRO, or COO.
* **Funding:** Series rounds or acquisitions.
* **Major Outages:** Significant downtime reported by users.

## 3. Output Trigger
Run this scan daily.

### Output Template: COMPETITIVE INTEL
**⚠️ RADAR HIT: [Competitor Name]**
* **Event:** [Type, e.g., C-Level Hire]
* **Details:** [Summary of the news]
* **Impact Assessment:** [Low/Medium/High risk to Lambda Test]
