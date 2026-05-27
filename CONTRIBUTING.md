# Contributing to Psychohistory in the Age of AI

Thank you for your interest in this project. This is an open research initiative — no institutional affiliation required, no minimum contribution size, no gatekeeping. If you find something interesting here and want to push it forward, you are welcome.

---

## Who Should Contribute

This project sits at the intersection of several fields. You do not need to cover all of them — partial expertise is fine.

**Useful backgrounds:**
- Computational social science
- Complex systems / dynamical systems
- Economic history or historical sociology
- Data science and time-series analysis
- Agent-based modeling
- Network science
- Political science with quantitative methods
- Physics (the wave models translate directly)
- Anyone with patience for messy historical data

**Students especially welcome.** This project is well-suited for a Master's thesis, a PhD chapter, or an undergraduate capstone. The framework is defined; the experimental work is open.

---

## Ways to Contribute

### 1. Data Curation
Pick one historical case from the [Research Proposal](RESEARCH_PROPOSAL.md) and build a clean dataset. This means:
- Identifying proxy data sources (see the Data Sources section of the proposal)
- Documenting reliability scores for each source
- Producing a clean CSV or similar format with a README explaining the variables
- Noting gaps, inconsistencies, and known biases

This is unglamorous work and extremely valuable. Without clean data, none of the formulas can be tested.

### 2. Formula Implementation
Pick one of the twelve formulas and implement it in Python. This means:
- Writing the formula as a function with clearly named parameters
- Documenting what each parameter represents and how to estimate it from data
- Running it on at least one historical case
- Reporting what it gets right and what it gets wrong

Do not worry about making it perfect. A documented failure is more valuable than silence.

### 3. Backtesting
Run one or more formulas against the suggested historical cases and measure performance using AUC and Brier score. Report results honestly, including failures. Especially useful: identifying which parameters matter most by removing them one at a time and measuring the change in accuracy.

### 4. Failed-Forecast Analysis
Take any prediction the formulas make that is clearly wrong and write a short analysis of why. What variable was missing? What assumption failed? What new hypothesis does the failure suggest? This is how the models improve.

### 5. New Formula Variants
If you see a gap or weakness in the existing formulas, propose a variant. You do not need to prove it works — submit it with a clear statement of what problem it is trying to solve and what data would test it.

### 6. Literature Mapping
Map existing academic work in computational social science, cliodynamics, or complex systems onto this framework. What has already been empirically tested? Where does existing literature confirm or contradict the hypotheses in the Research Proposal?

### 7. Visualization
Build clear visualizations of the wave models, collapse/resilience trajectories, or parameter sensitivity results. Good charts help researchers see patterns that formulas obscure.

---

## How to Submit

### For small contributions (datasets, charts, analysis):
1. Fork the repository
2. Add your files to a clearly named folder: `experiments/your-case-name/`
3. Include a README in your folder explaining what you did, what data you used, and what you found
4. Submit a Pull Request

### For discussions and proposals:
Open an Issue. Describe:
- What you plan to work on
- What approach you intend to take
- What you need (data, feedback, a second pair of eyes)

### For literature references:
Add them to `REFERENCES.md` (create it if it does not exist yet) with a one-sentence note on relevance.

---

## File and Folder Conventions

```
experiments/
  rome-collapse/
    README.md          ← what you did and what you found
    data/              ← raw and cleaned datasets
    notebooks/         ← Jupyter notebooks
    results/           ← outputs, charts, scores
  japan-resilience/
    ...
formulas/
  gemini_formula.py
  deepseek_formula.py
  ...
data/
  shared/              ← datasets useful across multiple cases
```

---

## Standards

**Honesty over optimism.** Report failures as carefully as successes. A formula that fails in an interesting way is more useful than silence.

**Document your data.** Every dataset should include its source, how it was cleaned, and what its known limitations are.

**Reproducibility.** Notebooks should run from top to bottom without manual intervention. Pin your library versions.

**No minimum.** A single well-curated dataset or a single documented failure is a real contribution.

---

## Acknowledgment

All contributors will be acknowledged in the project README. If a contribution leads to a publication, the contributing researcher will be included as a co-author — this is a commitment, not a courtesy.

---

## A Note from the Author

I am a retired computer engineer in Istanbul. I developed the conceptual framework for this project through conversations with twelve AI systems. The ideas are here. The experiments are not — because running them requires time, compute access, and institutional support that I do not have.

If you find this framework interesting and want to test it, please do. You do not need my permission. Fork it, break it, improve it. If you find something that works, tell me. If you find something that does not work, that is even more useful — tell me that too.

The goal is not to be right. The goal is to find out.

— Emin
