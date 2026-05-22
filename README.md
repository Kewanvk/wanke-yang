### Wanke Yang

Finance graduate with 5 years of management consulting at Mercer (Marsh McLennan). Now pursuing an MSc in Responsible Management at the University of Geneva.

I care about one thing in research: can someone else check your work? The projects below reflect how I approach this. Each one covers a different part of the research pipeline, from collecting raw data to producing a finished analysis to verifying that the conclusions actually hold up.

---

#### At a glance

| Project | Part of the pipeline | Output |
|---|---|---|
| [Financial data analysis](https://github.com/Kewanvk/smi-market-timing-analysis) | Analysis and reporting | Research memo, Python script, charts |
| [Structured data intelligence](https://github.com/Kewanvk/linkedin-recon-skill) | Data collection and structuring | Interactive reports, org maps, network graphs |
| [Research quality control](https://github.com/Kewanvk/zuoshi-kaopu) | Verification and challenge | Source-verified output with evidence trails |

---

### Part 1: Analysis and Reporting

**The question:** How much does market timing actually cost? The standard argument only shows one side. Does it survive a symmetric test?

**Data:** Swiss Market Index, daily returns, 2006 to 2025. Source: Yahoo Finance.

**Method:** Remove the N best days, the N worst days, or both. Compute compounded returns. Repeat across 16 rolling 5-year windows to check robustness.

**What I found:** The extreme up and down days cluster together. Missing both barely changes the outcome. The standard argument holds, but only after you test the other side.

**Limitations:** Uses price return index, not total return. No transaction costs. The conclusion (stay invested) is not new. The contribution is completing the symmetric case, not discovering something.

**What I would improve:** Re-run with total return data (Bloomberg SMIC) and add a transaction cost layer.

[View repository and full memo](https://github.com/Kewanvk/smi-market-timing-analysis)

---

### Part 2: Data Collection and Structuring

**The question:** Can you turn scattered public professional data into structured, actionable organizational insight?

**Data:** Public professional profiles collected via API. Hundreds of data points per analysis.

**Method:** Systematic collection, then multi-dimensional cross-analysis: role, seniority, tenure, connections, content activity, and relationship patterns. Framework-based, not ad hoc.

**What it produces:** Single-page interactive HTML reports with organizational structure visualization (SVG), relationship network mapping (D3.js), and prioritized recommendations.

**Limitations:** Quality depends on public data availability. Ethical constraints on data usage are documented and enforced in the codebase.

[View repository](https://github.com/Kewanvk/linkedin-recon-skill)

---

### Part 3: Verification and Challenge

**The problem:** AI-assisted research is fast but fragile. Models generate plausible text that may not be grounded in your actual sources. How do you catch this without slowing down?

**Solution:** Two independent actions, usable at any point during research.

*Brainstorm:* A second AI model receives your work and challenges it. Finds unstated assumptions, logical gaps, and unconsidered angles. Does not provide replacement solutions. You decide what to change.

*Verify:* NotebookLM searches your source documents and returns exact quotes, source locations, and confidence levels. If no evidence exists, it says "not found." No guessing.

**Limitations:** Brainstorm quality depends on the second model. Verification only works against uploaded documents, not the open internet.

[View repository](https://github.com/Kewanvk/zuoshi-kaopu)

---

### Background

- **Education:** BSc Finance (Southwestern University of Finance and Economics) / MSc Responsible Management (University of Geneva, current)
- **Experience:** 5 years management consulting at Mercer. Organizational change, knowledge systems, end-to-end client delivery across SOEs, multinationals, and private companies.
- **Tools:** Python (pandas, matplotlib), AI-assisted research workflows, structured reporting
- **Languages:** Chinese (native), English (fluent)
- **Location:** Geneva, Switzerland. Valid Swiss work permit.
