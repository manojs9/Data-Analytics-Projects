# 🧠 Multi-Agent Investment Advisory System (CrewAI + Google Gemini)

This project demonstrates how to build a **multi-agent investment advisory workflow** using  
**CrewAI**, **Google Gemini Flash**, and structured task dependencies.

It generates a complete investment advisory report using **five domain-specialized agents**:

---

## 👥 Agents

- **Market Analyst** – Analyzes equity, bonds, gold & macro trends  
- **Risk Specialist** – Evaluates investor risk profile  
- **Portfolio Engineer** – Designs diversified asset allocation  
- **Compliance Advisor** – Ensures SEBI-aligned recommendations  
- **Final Writer** – Compiles the finished advisory report  

---

## 🏗 Workflow Architecture

```mermaid
flowchart TD
    A[Market Analysis Task] --> C[Portfolio Construction]
    B[Risk Assessment Task] --> C
    C --> D[Compliance Check]
    A --> E[Final Writer]
    B --> E
    C --> E
    D --> E
'''

