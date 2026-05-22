### Wanke Yang

Finance graduate with 5 years of management consulting at Mercer (Marsh McLennan). Now pursuing an MSc in Responsible Management at the University of Geneva. I build Python workflows for evidence-based investment research, data quality control, and structured reporting.

---

#### What I have built

| Project | What it does | Output |
|---|---|---|
| [Financial data analysis](https://github.com/Kewanvk/smi-market-timing-analysis) | Tests a common investment claim against 20 years of Swiss market data. Documents assumptions, includes failure cases. | Python script, charts, research memo |
| [Structured data intelligence](https://github.com/Kewanvk/linkedin-recon-skill) | Collects raw data from public sources, applies multi-dimensional analysis, produces structured insight reports. | Interactive reports, org maps, relationship graphs |
| [Research quality control](https://github.com/Kewanvk/zuoshi-kaopu) | Two actions: adversarial review (a second model challenges blind spots) and source verification (checks claims against documents, returns exact quotes). | Verified research output with source trails |

---

#### Financial Data Analysis

**Question tested:** How much does market timing actually cost, and does the standard argument hold up when you test both sides?

**Data:** Swiss Market Index (SMI), daily returns, 2006 to 2025. Source: Yahoo Finance.

**Method:** Remove the N best days, the N worst days, or both from the return series. Compute compounded cumulative returns for each scenario. Repeat across rolling 5-year windows.

**Output:** Research memo with methodology, five data tables, three charts, and a reproducible Python script.

**Limitations:** Uses price return index, not total return. Does not include transaction costs. The practical conclusion (stay invested) is well established; the contribution is completing the symmetric argument, not discovering something new.

[View repository](https://github.com/Kewanvk/smi-market-timing-analysis)

---

#### Structured Data Intelligence

**Question tested:** Can you extract actionable organizational insight from scattered public professional data?

**Data:** Public professional profiles collected via API. Hundreds of data points per analysis.

**Method:** Systematic collection, multi-dimensional cross-analysis (role, seniority, tenure, connections, content activity), relationship mapping, structured report generation.

**Output:** Single-page interactive HTML reports with org structure visualization (SVG), hidden relationship networks (D3.js force graphs), and prioritized action plans.

**Limitations:** Dependent on public data availability. Analysis quality scales with data completeness. Ethical constraints on data usage are documented and enforced.

[View repository](https://github.com/Kewanvk/linkedin-recon-skill)

---

#### Research Quality Control

**Question tested:** How do you reduce hallucination and blind spots in AI-assisted research without slowing down?

**Method:** Two independent actions, usable at any point in a research workflow.
1. *Brainstorm:* A second AI model receives your work and challenges it. It finds unstated assumptions, logical gaps, and things you have not considered. It does not give replacement solutions.
2. *Verify:* NotebookLM searches your source documents for evidence supporting or contradicting each claim. Returns exact quotes, source locations, and confidence levels. If no evidence exists, it says "not found."

**Output:** Research output with documented challenge rounds and source-grounded verification trails.

**Limitations:** Brainstorm quality depends on the second model's reasoning ability. Verification only works against documents you have uploaded; it cannot check claims against the open internet.

[View repository](https://github.com/Kewanvk/zuoshi-kaopu)

---

#### Background

- **Education:** BSc Finance (Southwestern University of Finance and Economics, China) / MSc Responsible Management (University of Geneva, current)
- **Experience:** 5 years management consulting at Mercer, working with SOEs, multinationals, and private companies on organizational change, knowledge systems, and client delivery
- **Tools:** Python (pandas, matplotlib), AI-assisted research workflows, structured reporting
- **Languages:** Chinese (native), English (fluent)
- **Location:** Geneva, Switzerland. Valid Swiss work permit.
