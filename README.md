# vbp-ai-framework
## VBP-AI: The Open Source Value-Based Procurement Framework

### Version 1.0 | Industry Standard for Outcome-Linked AI Contracting

The traditional SaaS per-seat licensing model is dead because AI naturally reduces human headcount. Concurrently, consumption-based billing (paying per token) forces enterprise buyers to bear 100% of the vendor's raw infrastructure and inference inefficiencies.

The **VBP-AI Framework** is an open-source, vendor-agnostic procurement standard designed to shift the balance of power back to the buyer. It establishes a repeatable mechanism to buy AI capabilities based on **economic utility** while enforcing strict financial penalties for algorithmic errors.

---

## 1. The Core Architecture: Outcome-Linked Monetization

Under the VBP-AI standard, vendors are forbidden from charging for raw computational effort. Instead, they must map their commercial models into one of three verified **Value-Based Tiers**:

| Billing Model | Primary Metric | Target Use Cases | Financial Risk Profile |
| --- | --- | --- | --- |
| **Workflow / Task-Based** | Fee per successfully completed document, contract parsed, or ticket processed. | Structured data extraction, compliance screening, automated reporting. | **Shared Risk:** Vendor charges nothing if the model hits a fatal parsing error or formatting exception. |
| **Resolution / Success-Based** | Fee per verified business resolution (e.g., customer issue closed without human escalation). | Autonomous customer agents, IT helpdesk triaging, sales routing. | **High Vendor Risk:** Wasted tokens or circuitous reasoning paths are 100% absorbed by the vendor. |
| **Value-Capture / Shared ROI** | Percentage of verified cost savings or revenue generation (e.g., 10% of recovered SaaS spend variance). | Procurement optimization, autonomous contract renegotiation. | **Symmetrical Alignment:** Revenue scales directly with the actual economic value delivered to the buyer. |

---

## 2. The Hallucination & Abstention Accounting Protocol (The "SLA Model")

To institutionalize a culture where vendors do not profit from misinformation, the framework introduces three mandatory legal clauses to be appended to all Master Services Agreements (MSAs) and RFPs.

### Clause A: The Zero-Rating for Intrinsic Hallucinations

> **Contractual Language Boilerplate:**
> *"The Buyer shall incur zero ($0.00) financial liability for any transaction, output, or API response containing an Intrinsic Hallucination. An Intrinsic Hallucination is defined as any model output that introduces, fabricates, or expands upon facts, data points, or parameters that cannot be structurally derived from the provided grounded context documents (RAG) or the user's explicit system instructions."*

### Clause B: The "Silence Credit" (Abstention Protection)

If an AI agent cannot answer a query because your internal documentation is incomplete, it has performed correctly by choosing silence over fiction.

* Vendors cannot charge for the tokens used to generate an explicit refusal (e.g., *"I do not have sufficient verifiable data to execute this"*).
* Removing the financial penalty for abstention actively protects your business from forced, confident hallucinations.

### Clause C: Inference-Chain and Reasoning Token Exclusions

Advanced reasoning models (such as OpenAI's o-series or DeepSeek-R1) generate thousands of hidden "thinking tokens" during reinforcement-learning execution loops.

* **The VBP-AI Rule:** Enterprise buyers pay strictly for input tokens and final, customer-facing output tokens. Internal logical divergence, infinite reasoning loops, or recursive system prompts are entirely a product optimization cost for the vendor to absorb.

---

## 3. The Automated Billing Verification Pipeline

You cannot enforce value-based contracts using manual human audits. The VBP-AI framework mandates an automated, programmatic telemetry stack to settle monthly invoices.

```
                  ┌──────────────────────────────┐
                  │      User API Transaction    │
                  └──────────────┬───────────────┘
                                 ▼
                  ┌──────────────────────────────┐
                  │    Primary AI Model Output   │
                  └──────────────┬───────────────┘
                                 ▼
                  ┌──────────────────────────────┐
                  │  Independent Judge Layer     │
                  │  (Vectara HHEM / Galileo)    │
                  └──────────────┬───────────────┘
                                 ▼
         ┌───────────────────────┴───────────────────────┐
         ▼                                               ▼
[Factual Score ≥ 95%]                           [Factual Score < 95%]
• Passed to Production                           • Automatically Blocked
• Logged as "Billable"                          • Logged as "Zero-Rated"

```

The buyer deploys a lightweight, independent evaluation layer (such as Vectara's open HHEM model) at the API gateway. Every response is dynamically assessed for factual consistency. If the consistency score drops below a contractually agreed baseline (e.g., 95% consistency), the transaction ID is programmatically flagged on the ledger as non-billable.

---

## 4. Implementation Sequence for Sourcing Teams

To roll out the VBP-AI framework within your organization's sourcing and tech onboarding workflows, follow this implementation path:

1. **Step 1: Segment Workflows by Value Horizon:** Days 1-15.
Audit your current AI vendor pipeline. Identify which deployments are "Soft ROI" (e.g., an internal assistant that summarizes emails) versus "Hard ROI" (e.g., an autonomous agent automating vendor risk monitoring). Target the Hard ROI workflows for immediate value-based pricing conversion.


2. **Step 2: Append the VBP-AI Addendum to RFPs:** Days 16-30.
Insert the standardized VBP-AI clauses directly into incoming vendor RFPs. Force vendors to declare their baseline Intrinsic Hallucination rate and explicitly state how they intend to handle the financial cost of ungrounded or failed outputs.


3. **Step 3: Establish the Independent Judge Gateway:** Days 31-45.
Deploy a third-party evaluation model within your internal infrastructure. This layer acts as your neutral financial auditor, checking the outputs of enterprise vendors against your source documents before billing logs are synced.


4. **Step 4: Execute the Risk-Share Reconciliation:** Ongoing.
Review your automated billing logs during monthly vendor syncs. Deduct flagged hallucinations and abstention overheads directly from the invoice statement, creating a direct financial feedback loop that encourages the vendor to optimize for accuracy.


---

## Public Distribution & License (MIT)

The VBP-AI Procurement Framework is released under the **MIT Open Source License**. It is conceived and incepted by Mr. Sandeep Joshi at Protum.ai. Any enterprise, procurement group, or technology consortium is permitted to copy, modify, merge, and distribute these templates without restriction. The goal is simple: collectively raising the bar for AI quality by forcing vendors to stand financially behind the performance of their models.

