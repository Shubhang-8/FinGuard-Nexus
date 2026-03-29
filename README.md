#  FinGuard-Nexus
### **Enterprise Multi-Agent Compliance & Audit Engine**
*Final Submission for ET Hackathon Phase 2*

FinGuard-Nexus is a high-precision AI orchestrator designed to automate the **Financial Close** and **AML/SAR Reporting** workflows. By utilizing a specialized Multi-Agent architecture, it eliminates manual reconciliation errors and ensures 100% auditability in regulatory filings.

---

##  Core Architecture (The Multi-Agent System)
FinGuard-Nexus operates through three autonomous agents powered by **Claude 3.5 Sonnet**:

1. **Integrity Agent (Mathematical Audit):** Performs real-time reconciliation of the transaction ledger. It identifies "Reconciliation Gaps" by dynamically auditing Total Credits vs. Total Debits.
2. **Forensic Agent (Pattern Detection):** Scans for complex criminal typologies including **Structuring** (31 CFR 1010.311) and **Layering** (Pass-through wires).
3. **Governance Agent (The Hallucination Shield):** Our proprietary safety layer. It cross-verifies every sentence of the generated SAR against raw Ledger Row IDs to ensure zero hallucinations.

---

## Key Features & Impact
- **Dynamic Ingestion:** Judges can upload any banking CSV to trigger a live system audit.
- **Hallucination Shield:** Real-time verification status for all subject names and transaction amounts.
- **Regulatory Readiness:** Generates structured, copy-to-clipboard SAR narratives for direct FinCEN portal entry.
- **99.8% Cost Efficiency:** Reduces manual SAR generation from 6 hours ($300 analyst cost) to 60 seconds ($0.50 API cost).

---

## Setup & Local Execution
1. Clone the repository: `git clone https://github.com/Shubhang-8/FinGuard-Nexus.git`
2. Install dependencies: `pip install -r requirements.txt`
3. Run the application: `streamlit run app.py`

*Note: Ensure your `.env` file contains a valid `ANTHROPIC_API_KEY` to initialize the agents.*
