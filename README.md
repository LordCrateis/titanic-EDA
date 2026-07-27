# Titanic Dataset: Contextual & Spatial EDA

> **Project Goal:** Moving beyond standard statistical summaries to extract historical, spatial, and social constraints from the Titanic dataset for downstream choice-based game mechanics and contextual ML models.[cite: 1]

---

### Key Narrative Insights & Feature Engineering

1. **Spatial Vulnerability (Class vs. Deck Placement)**
   * **Finding:** 3rd Class passengers faced ~70% mortality.[cite: 1]
   * **Context:** First-class cabins were near the boat deck; third-class/steerage was at the bottom/stern.[cite: 1] Physical distance to lifeboats dictated survival before decision-making even began.[cite: 1]

2. **The "Solo Male" Casualty Spike**
   * **Feature Created:** `ptype` (`Individual` vs. `Family`).[cite: 1]
   * **Finding:** Solo travelers suffered massive casualty rates, overwhelmingly male, while traveling with family significantly increased survival odds for women/children due to social/evacuation protocols.[cite: 1]

---

### Key Visualizations
![Class Survival Breakdown](./assets/pclass_survival.png)
![Deck Layout](./assets/titanic_ship_deck.png)

---

### Tech Stack & Methods
* **Analysis:** Python (`pandas`, `numpy`)[cite: 1]
* **Visualization:** `seaborn`, `matplotlib`[cite: 1]
* **Feature Engineering:** Binning age brackets, merging relational metadata, engineered `ptype` (Individual/Family split).[cite: 1]