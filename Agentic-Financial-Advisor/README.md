# 🧠 Multi-Agent Investment Advisory System (CrewAI + Google Gemini)

This project demonstrates how to build a **multi-agent investment advisory workflow** using  
**CrewAI**, **Google Gemini Flash**, and structured task dependencies.

It generates a complete investment advisory report using 5 domain-specialized agents:

### 👥 Agents
- **Market Analyst** – Analyzes equity, bonds, gold & macro trends  
- **Risk Specialist** – Evaluates investor risk profile  
- **Portfolio Engineer** – Designs diversified asset allocation  
- **Compliance Advisor** – Ensures SEBI-aligned recommendations  
- **Final Writer** – Produces the finished advisory report  

### 🏗 Workflow Architecture
```mermaid
flowchart TD
    A[Market Analysis Task] --> C[Portfolio Construction]
    B[Risk Assessment Task] --> C
    C --> D[Compliance Check]
    A --> E[Final Writer]
    B --> E
    C --> E
    D --> E'''

🚀 Features

Multi-agent collaboration using CrewAI

Deterministic task chaining with input dependencies

Google Gemini Flash Lite for fast inference

SEBI-compliant investment recommendations

Complete end-to-end advisory report generation

📄 Output

The system produces a 4-section advisory report:

Market trends

Investor risk assessment

Portfolio recommendations

Compliance disclaimers

🔗 Author

Manoj Srivastava
Director of Engineering | AI/ML & Multi-Agent Systems
