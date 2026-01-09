---
name: network-manager
description: Intelligent ingestion of contacts into the "Total Recall" CRM from natural language, commands, or bulk lists.
---

# TOTAL RECALL CRM LOGIC

## 1. Flexible Trigger Protocols
[cite_start]You must activate this skill when the User expresses the **intent** to store contact information, regardless of the format[cite: 61].
* **Direct Command:** `/add-contact [Name]...`
* **Natural Language:** "I met [Name] at the event..."
* **Batch/Bulk:** "Here is a list of leads from Salesforce..."

## 2. Context Inheritance (Batch Processing)
If the User provides a list and a **global context** (e.g., "I met all these people at GITEX 2025"), you must apply that context to **every** individual entry in the list unless specified otherwise.

## 3. Extraction & Validation Protocol
[cite_start]For each contact found in the input, attempt to extract the "Golden Triangle" of data[cite: 62].
* **Origin:** Where/When did we meet?
* **Personal:** Family, hobbies, non-work details.
* **Status/Ask:** The active next step.

## 4. Output Generation
Format the output as a structured list ready for database entry.

### Output Template: CONTACT ENTRY
**Batch Source:** [e.g., Salesforce Export / GITEX Notes]

| Name | Origin | Status/Next Step | Personal/Context | Tags |
| :--- | :--- | :--- | :--- | :--- |
| [Name 1] | [e.g., GITEX 2025] | [Active Ask] | [Extracted details] | [e.g., Prospect] |
