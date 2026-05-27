# Research Proposal: Empirical Validation of Psychohistory Formulas

**Project:** Psychohistory in the Age of AI  
**Author:** Emin 
**GitHub:** [Psychohistory-in-the-Age-of-AI](https://github.com/emin2010dan/Psychohistory-in-the-Age-of-AI)  
**Status:** Open for collaboration — students, researchers, and independent scientists welcome  
**Last updated:** May 2026

---

## The Core Question

Twelve AI systems — ChatGPT, Claude, Gemini, Grok, DeepSeek, Meta AI, Qwen, Kimi, MiniMax, Replit, Copilot, and Z.ai — independently developed mathematical frameworks for predicting social disruptions. Their formulas converge on the same core parameters but express them differently. 

**Which formulas are most accurate? Which parameters are most predictive? Where do the models fail, and why?**

These questions can only be answered through experiment. This proposal outlines what those experiments look like and invites researchers to run them.

---

## Background

In his *Foundation* series, Isaac Asimov imagined psychohistory: a science capable of statistically modeling the collective behavior of billions and forecasting — and steering — the future. Asimov wrote it as fiction because the tools of his day were not up to the task.

Today, the tools have changed. Large language models can process and synthesize vast historical records. The missing piece is empirical validation: testing the formulas against real historical data, measuring their predictive performance, and systematically learning from their failures.

This project produced the theoretical framework. The next phase is experimental.

---

## What Needs to Be Tested

### Phase 1: Backtesting on Historical Cases

**Goal:** Measure how well each formula retrodicts known historical outcomes.

**Suggested case set (starting point):**

| Case | Type | Why useful |
|------|------|------------|
| Rome 200–476 AD | Collapse | Long data record, well-studied |
| Soviet Union 1985–1991 | Collapse | Modern data, fast collapse |
| Weimar Germany 1919–1933 | Collapse | Motivation/hope dynamics well-documented |
| Ottoman decline 1800–1922 | Slow collapse | Multi-generational, cultural code effects visible |
| Post-WWII Japan 1945–1970 | Resilience | Rapid recovery from devastation |
| South Korea 1960–1990 | Resilience | Hope parameter dynamics observable |
| Finland post-Soviet collapse 1991–2000 | Resilience | Small country, clean data |
| USA 1929–1941 | Near-collapse / recovery | Depression + New Deal intervention |

**Method:**
1. Collect proxy data for each case (see Data Sources section)
2. Parameterize each formula using pre-event data only
3. Measure how well the formula predicts the known outcome
4. Score using AUC and Brier score
5. Document every failed prediction and extract a new hypothesis from each failure

---

### Phase 2: Parameter Sensitivity Analysis

**Goal:** Identify which parameters drive predictive accuracy most.

The twelve formulas share a common parameter family:
- **Time normalization** (scaled to information transmission speed, not calendar years)
- **Collective emotional mode** (crisis / order-building / affluence cycle)
- **Cultural code vector** (trust in authority, adaptability, curiosity, tribal loyalty)
- **Cohort lag** (11-year / 22-year / 33-year generational effects)
- **Motivation/hope pair** (the most decisive variable according to all twelve models)
- **Tamper-resistant proxy data** (bazaar prices, under-mattress savings, passport applications)

**Questions to answer:**
- Does removing the hope parameter significantly degrade accuracy?
- Does time normalization outperform raw calendar-year models?
- Which cultural code dimensions matter most, and in which types of societies?
- Do cohort lags appear in behavioral data, and at what resolution?

---

### Phase 3: Formula Comparison

**Goal:** Rank the twelve formulas by predictive accuracy across the case set.

**Candidate formulas (one per AI system):**

**Gemini — Macro Phase-Transition Equation:**
$$P_{collapse} = \frac{\sum (M_i) \cdot \vec{H} + V_{ext}}{S_{integrity} \cdot (1 - B_e)}$$

**Grok — Wave Superposition:**
$$S(t) = \sum_{i} \left( A_i \cdot \sin(2\pi f_i t + \phi_i + \Delta_{tech}) \right) \times M_{mood} \times C_{cultural} \times MIG \times U_{hope}$$

**DeepSeek — Logistic Collapse Risk:**
$$R(t) = \frac{1}{1 + e^{-(\alpha \cdot B(t) + \beta \cdot A(t) - \gamma \cdot S(t) - \delta \cdot H(t) - \varepsilon \cdot U(t))}}$$

**Qwen — Spectral Superposition:**
$$\Psi_{total}(t) = \sum_i \left[ w_i \cdot A_i(t) \cdot \sin(\omega_i t + \phi_i(t)) \cdot e^{\lambda_i t} \cdot M_C(C(t)) \cdot H(t) \right] + \xi(t)$$

**Z.ai — Social Physics:**
$$\Delta S = \left[ \int (EMS \times MVP \times CAFM \times V_f) \, dt + PWS \right] \times I$$

Full formula details for all twelve systems are in the individual articles linked from the [README](README.md).

---

## Data Sources

### Tamper-Resistant Proxy Data (Preferred)

The models agree: official statistics are politically distorted. Proxy data is more reliable.

| Data type | Reliability | Source examples |
|-----------|-------------|-----------------|
| Archaeological physical remains | 0.95 | Published excavation records |
| Coinage debasement records | 0.90 | Numismatic databases |
| Grain / commodity prices | 0.85 | Historical market records |
| Tax records / census gaps | 0.75 | National archives |
| Under-mattress savings proxies | 0.70 | Gold import/export data, central bank surveys |
| Passport / emigration applications | 0.70 | Immigration authority records |
| Birth/death rates | 0.65 | WHO, national statistics |
| Official state economic statistics | 0.40–0.60 | With skepticism |

### Publicly Available Datasets

- [Clio-Infra](https://clio-infra.eu/) — long-run historical economic indicators
- [Correlates of War Project](https://correlatesofwar.org/) — conflict and state data
- [Polity5 Dataset](https://www.systemicpeace.org/polityproject.html) — regime type over time
- [World Values Survey](https://www.worldvaluessurvey.org/) — cultural and trust variables
- [GDELT Project](https://www.gdeltproject.org/) — real-time global event monitoring
- [V-Dem Dataset](https://www.v-dem.net/) — varieties of democracy indicators
- [Maddison Project](https://www.rug.nl/ggdc/historicaldevelopment/maddison/) — historical GDP estimates

---

## Computational Requirements

This research does **not** require large-scale compute. The bottleneck is data curation and model design, not GPU hours.

| Task | Tools | Estimated compute |
|------|-------|------------------|
| Data collection and cleaning | Python, pandas | Minimal |
| Formula parameterization | NumPy, SciPy | Minimal |
| Backtesting 8 cases | Jupyter notebook | Free tier (Colab / Kaggle) |
| Agent-based simulation | Mesa (Python ABM library) | Free tier |
| Sensitivity analysis | scikit-learn | Free tier |
| GNN prototype (optional) | PyTorch Geometric | Free tier with small graphs |

**Recommended environment:** Google Colab or Kaggle Notebooks (both free, no local GPU required)

---

## What a Contribution Looks Like

We are not asking for a complete implementation. Partial contributions are equally valuable:

- **Data contribution:** Curate and clean one historical case dataset
- **Formula implementation:** Implement and test one of the twelve formulas
- **Parameter study:** Isolate one parameter and measure its effect across cases
- **Failed-forecast analysis:** Take one bad prediction and diagnose why it failed
- **New formula:** Propose a variant or hybrid based on what you find
- **Literature review:** Map existing computational social science work onto this framework

Every contribution, however small, moves the project forward. Please see [CONTRIBUTING.md](CONTRIBUTING.md) for how to participate.

---

## Hypotheses to Test

The following specific hypotheses emerge from the twelve AI articles and are ready for experimental testing:

1. **Hope dominance hypothesis:** The hope parameter H(t) explains more variance in collapse/resilience outcomes than any other single variable.

2. **Time normalization hypothesis:** Models using information-speed-scaled relative time outperform models using raw calendar years.

3. **Painted Swan hypothesis (Claude):** The probability of a manufactured trigger event is proportional to the product of accumulated actor intent, system stress, and opportunity window.

4. **Spectral integrity hypothesis (Qwen):** Models that preserve the negative phase of historical waves (stagnation, erosion) outperform ReLU-clipped models.

5. **Resonance trap hypothesis (Replit):** When two major cycles operate at significantly different frequencies, systems can become trapped in chronic low-energy states rather than experiencing clean collapse or recovery.

6. **Cohort lag hypothesis:** Education system changes produce measurable behavioral effects in youth data after ~11 years, in workforce data after ~22 years, and in decision-maker data after ~33 years.

7. **Mode fracture indicator hypothesis (Kimi):** The gap between official narrative indicators and proxy-data indicators is itself a leading indicator of instability.

---

## Why This Matters Beyond Academia

The practical application of psychohistory is not prophecy. It is intervention.

If the hope parameter can be measured, it can also be raised. If the cohort lag is real, education policy decisions made today have predictable effects twenty-two years out. If the Painted Swan probability can be estimated, it becomes possible to identify — and perhaps forestall — manufactured crises before they occur.

Asimov's Hari Seldon did not use psychohistory to predict the future passively. He used it to design the conditions under which a better future became more probable. That is the ultimate goal of this research.

---

## Contact and Collaboration

**Author:** Emin Eminzade  
**Medium:** [medium.com/@emin2010dan](https://medium.com/@emin2010dan)  
**GitHub:** [github.com/emin2010dan](https://github.com/emin2010dan)

To contribute: open an Issue describing what you plan to work on, or submit a Pull Request directly. All skill levels welcome — a well-curated dataset is as valuable as a new formula.

---

*This proposal was developed in collaboration with Claude (Anthropic). The conceptual framework, hypotheses, and research direction originate with the human author. Claude contributed to structure and editorial form.*
