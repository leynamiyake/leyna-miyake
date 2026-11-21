# Prompt Log

A record of prompts used to create, analyze, document, or improve projects in
this portfolio.

Keeping a prompt log helps document the development process and makes it easier
to reproduce useful AI-assisted workflows.

---

## Prompt Entry Template

### Stage 0

**Project name:**  
FX Hedging Prompt Stage 0 
**Date:**  
<!-- 2026-10-2 -->

**Purpose:**  
< Stage 0 focused on initializing the repository and setting up the foundational architecture for the project. The main goal was to establish the basic folder structure (analysis, data, docs), configure essential documentation files like README.md, CLAUDE.md, and prompt_log.md, and set up the Git repository on GitHub to prepare for future development and AI-assisted workflows.  -->

## Prompt Entry Template

### Stage 1

**Project name:**  
FX Hedging Prompt Stage 1
**Date:**  
<!-- 2026-10-15 -->
**Date:** October 29, 2026

**Prompt Used:** I asked AI to help me write a 400–600-word executive brief for my FX Hedging project using Scenario 17. I requested an explanation of the foreign exchange risk, a comparison of forward contracts, money-market hedges, and currency options, and a discussion of assumptions, hypotheses, and next steps.

**AI Output:** AI helped create an executive brief explaining how a U.S. server manufacturer faces exchange rate risk from a EUR 17,500,000 receivable due in 182 days. It described the advantages and disadvantages of three hedging strategies and provided a hypothesis about their expected results.

**Verification:** I reviewed the calculations showing how changes in the EUR/USD exchange rate affect the company's U.S. dollar proceeds. I also checked that the brief included the required hedging alternatives, assumptions, hypothesis, and project roadmap.

**Reflection:** Using AI helped me better understand foreign exchange exposure and how different hedging strategies can protect a company's cash flow. I learned that forward contracts provide certainty, money-market hedges use borrowing and investing, and options provide protection while allowing potential gains. AI was useful for organizing my ideas and explaining financial concepts clearly.


### Stage 3
**Project name:**  
FX Hedging Prompt Stage 3
**Date:**  
<!-- 2026-11-13 -->
**Purpose:**  
Prompt 1 — Understanding the Model Requirements
Purpose: I used AI to help me understand the Stage 3 requirements and how to apply my Stage 2 specification to an Excel workbook.

AI Assistance: AI helped explain the workbook structure, required calculations, named ranges, and validation checks. I used this guidance along with my Stage 2 specification to understand how the different hedging strategies should be organized.

Prompt 2 — Excel Model Development
Purpose: I used AI to assist with building the Excel workbook based on my Stage 2 specification.

AI Assistance: AI generated an initial Excel workbook using the formulas and assumptions outlined in my specification. I reviewed the workbook to better understand how the forward contract, money-market hedge, and currency put option calculations worked.

Prompt 3 — Reviewing Calculations and Troubleshooting
Purpose: I wanted to check whether the workbook calculations were consistent with my original specification.

AI Assistance: AI helped explain the results of the three hedging strategies and identify potential issues. I evaluated what I needed to change on the excel workbook.


Prompt 4 — Build Audit Analysis
Purpose: I used AI as a reference to help organize my audit findings and understand how to document the results.

AI Assistance: AI helped explain the importance of checking formulas, assumptions, sensitivity analysis, and formatting. I reviewed the identified issues and documented the observations in my Stage 3 audit report. I also used AI to help me craft the audit report so that it flows and sounds professional.

### Stage 4
**Market Data + Population:**  
FX Hedging Prompt Stage 4
**Date:** November 20, 2026

**Prompt Used:** I asked AI to update my Stage 3 Excel workbook, recalculating the sensitivity analysis, checking covered interest parity, and comparing the results with the FX Hedging Lab.

**AI Output:** AI updated the workbook using an EUR/USD spot rate of 1.0990, a USD interest rate of 3.91%, and a EUR interest rate of 2.441%. It recalculated the hedging strategies, updated the sensitivity analysis, and created a market-data memo documenting the sources and calculations.

**Verification and Corrections:** The workbook's formulas and named ranges were checked. The parity check showed a $1,110,158.85 difference between the forward and money-market hedges. Rather than changing the inputs to force the check to pass, the discrepancy was documented. The FX Hedging Lab's published formulas were compared with the workbook.

**Reflection:** AI helped me update the financial model and identify discrepancies in the hedging calculations. I learned the importance of documenting market-data sources, checking formulas, and explaining differences instead of adjusting numbers to get the expected results.
