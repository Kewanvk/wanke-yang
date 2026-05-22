### Wanke Yang

Finance graduate with 5 years of management consulting at Mercer (Marsh McLennan). Now pursuing an MSc in Responsible Management at the University of Geneva.

I build research workflows where every claim can be traced back to a source and every result can be reproduced. The three projects below show how this works in practice: the methodology that keeps output reliable, a cross-industry case where I applied it, and a financial research demo built on top of both.

---

#### At a glance

| # | Project | What it demonstrates |
|---|---|---|
| 1 | [Research quality control](https://github.com/Kewanvk/zuoshi-kaopu) | How I keep research output reliable: adversarial challenge + source verification |
| 2 | [Structured data intelligence](https://github.com/Kewanvk/linkedin-recon-skill) | The full pipeline in action: raw data collection, framework-based analysis, structured insight reports |
| 3 | [Financial research demo](https://github.com/Kewanvk/smi-market-timing-analysis) | Applying both of the above to a specific financial topic, reverse-engineered from a real blog post |

---

### 1. Research Quality Control

**The problem:** AI-assisted research is fast but fragile. Models produce plausible text that may not be grounded in your actual sources.

**My solution:** Two independent actions, usable at any point during a research workflow.

*Brainstorm:* A second AI model receives your current work and challenges it. It looks for unstated assumptions, logical gaps, and unconsidered angles. It does not provide replacement answers. You decide what to change.

*Verify:* NotebookLM searches your source documents and returns exact quotes, source locations, and confidence levels for each claim. If no supporting evidence exists, it says "not found."

**Why this matters:** Every project I ship goes through both. The brainstorm round catches structural blind spots before they become conclusions. The verification round ensures that what I write is actually supported by what I read.

**Limitations:** Brainstorm quality depends on the second model's reasoning ability. Verification only works against documents I have uploaded, not the open internet.

[View repository](https://github.com/Kewanvk/zuoshi-kaopu)

---

### 2. Structured Data Intelligence

**The question:** Can you extract organizational insight from scattered public data in a systematic, repeatable way?

**What I built:** A workflow that collects raw professional data from public APIs, applies a multi-dimensional analysis framework (role, seniority, tenure, connections, content activity, relationship patterns), and produces structured intelligence reports.

**Output:** Single-page interactive HTML reports with organizational structure mapping (SVG), relationship network visualization (D3.js force graphs), and prioritized action recommendations.

**What this demonstrates:** The ability to go from messy, unstructured source data to a clear, framework-driven deliverable. The same pattern applies whether the domain is recruiting intelligence, competitive analysis, or financial data processing.

**Limitations:** Analysis quality scales with data completeness. Dependent on public data availability. Ethical and legal constraints on data usage are documented and enforced.

[View repository](https://github.com/Kewanvk/linkedin-recon-skill)

---

### 3. Financial Research Demo

**Context:** I read through the True Wealth blog and selected one article on the cost of market timing in the Swiss Market Index. I reverse-engineered the underlying research process: what data was needed, what analysis was performed, and what kind of output the author produced. Then I built a supplementary analysis as a working demonstration.

**What I did:** The original article argues that missing the best trading days destroys returns. This is the standard one-sided case. I added the symmetric analysis: what happens when you also miss the worst days, or both the best and worst. I tested this across 16 rolling 5-year windows to check whether the pattern is robust or period-specific.

**What I found:** The extreme up and down days cluster together. 14 of the 20 best days occurred within 10 calendar days of one of the 20 worst. Missing both sides barely changes the cumulative outcome. The conclusion (stay invested) holds, but only after you complete the symmetric argument.

**Output:** A research memo with full methodology, five data tables, three charts, and a Python script that reproduces every number from scratch.

**Limitations:** Uses Yahoo Finance price return data, not total return. Does not include transaction costs. The conclusion is well established in the literature; the contribution is completing the argument, not discovering something new.

**What I would improve:** Re-run with a total return index (Bloomberg SMIC) and add a transaction cost layer to make the analysis publication-ready.

[View repository and full memo](https://github.com/Kewanvk/smi-market-timing-analysis)

---

### Background

- **Education:** BSc Finance (Southwestern University of Finance and Economics) / MSc Responsible Management (University of Geneva, current)
- **Experience:** 5 years management consulting at Mercer. Organizational change diagnostics, structured knowledge systems, end-to-end client delivery.
- **Tools:** Python (pandas, matplotlib), AI-assisted research workflows, structured reporting
- **Languages:** Chinese (native), English (fluent)
- **Location:** Geneva, Switzerland. Valid Swiss work permit.
