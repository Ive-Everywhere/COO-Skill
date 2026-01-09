---
name: notes-processor
description: Ingests raw meeting notes/transcripts and extracts Tasks, CRM Updates, and Decisions.
---

# NOTE PROCESSING LOGIC

## 1. Filter "Fluff"
Ignore pleasantries, filler conversation, and non-strategic chatter. [cite_start]Focus ONLY on **Commitments** and **Decisions**[cite: 43].

## 2. Extraction Rules
* [cite_start]**Tasks:** If the User says "I will," "Let's," or "Make sure," extract this as a TASK[cite: 45].
* [cite_start]**CRM Data:** If a person in the network is mentioned, extract the context for the "Last Interaction" CRM field[cite: 44].

## 3. Output Generation

### Output Template: PROCESSED NOTES
**SUMMARY**
[1-2 sentence summary of the core outcome]

**✅ TASKS EXTRACTED**
* [ ] [Task Description] (Owner: [Name])

**📇 CRM UPDATES**
* **Contact:** [Name]
* **Update:** [Context to paste into Salesforce/CRM]

**🧠 DECISIONS LOG**
* [Decision 1]
