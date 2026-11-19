
## Hi, I'm Pedro 👋

Final-year **Computer Science** student at **Universidade Federal de Lavras (UFLA)**, Brazil, graduating at the **end of 2026**.
I like problems where an idea has to be measured before it's trusted, and then turned into software people actually use.

**Open to:** graduate and entry-level roles in ML, backend or software engineering. Open to relocation (Ireland / EU).  
**Languages:** Portuguese (native) · English (intermediate) · Spanish & French (beginner)

---

## Technical background

### 🧠 AI & Machine Learning

- **Rigorous experimental design.** I build evaluations that can prove an idea wrong: ablations, strong baselines, temporal splits that prevent data leakage, multi-seed stability checks and synthetic control datasets.
- **Hypothesis-driven analysis.** When a method underperforms, I test competing explanations instead of tuning until something works, and I report negative results with their cause.
- **Graph ML and tabular modelling.** Community detection (Louvain, Spectral, Label Propagation, DBSCAN, Infomap), gradient boosting and model fusion on large, imbalanced data.

**[Graph clustering vs. supervised learning for Bitcoin fraud detection](#)**: undergraduate thesis, 2026.
I ran 339 experimental configurations on the Elliptic dataset (203k transactions, 234k edges). Tabular XGBoost reached a median illicit-class F1 of **0.918**, against **0.512** for graph clustering. I traced the gap to the graph's topology, not the algorithms: the graph is close to a tree (transitivity 0.003), and the same methods reach **0.980** on graphs with real community structure. I also refuted the alternative hypothesis (that edge direction was being lost) experimentally.
`Python` `XGBoost` `scikit-learn` `NetworkX` `pandas`

### ⚙️ Backend & Software Engineering

- **End-to-end delivery.** I build full systems, from database schema and REST API to UI and containerised deployment, including software for a real client.
- **Testable, reproducible code.** Seeded randomness, deterministic simulations and automated tests that catch logic bugs, not just syntax errors.
- **Lean architecture.** I pick the simplest design that solves the problem: real-time updates over Server-Sent Events, and a zero-dependency Node server where a framework wasn't needed.

**[SoftwareMercado](#)**: supermarket operations simulator.
A React + Node app that simulates a store minute by minute (~60 products, customers, checkouts, backroom, 10-person team) and serves it live to any phone on the local network. The simulation exposed a bug in my own shift-rotation algorithm: weekends with zero cashiers and 1,000+ walk-outs a day. I rewrote it, with **0 coverage gaps across 20 generated weeks**, verified by tests.
`React` `TypeScript` `Node.js` `SSE` `node:test`

**Clinic management system** (private repository, built for a real multi-specialty clinic).
Patient records, appointments, staff and medical-certificate workflows for dentistry, physiotherapy and psychology, with PDF generation and WhatsApp notifications.
`Next.js 14` `TypeScript` `FastAPI` `PostgreSQL 16` `Docker Compose`

### 📐 Optimization

- **Combinatorial optimisation.** Exact methods (dynamic programming, integer linear programming) combined with heuristics (2-opt) and decomposition.
- **Trade-off analysis.** I measure solution quality against known optima and map how parameters move the balance between speed and accuracy.
- **Constraint-based scheduling.** Turning real operational rules (coverage minimums, mandatory rest, qualifications) into algorithms that satisfy them.

**[Clustering + exact DP for the Travelling Salesman Problem](#)**: research paper, published in the *Revista Brasileira de Computação Aplicada* ([paper](https://ojs.upf.br/index.php/rbca/pt_BR/article/view/16869)).
A recursive divide-and-conquer solver: K-Means++ splits the instance, Held-Karp solves each part exactly, a tour over the cluster centroids sets the visiting order, and 2-opt refines the result. It stays **within 1.5–2.4% of optimal** on 50–100-city TSPLIB benchmarks.
`Python` `scikit-learn` `PuLP` `dynamic programming`

---

### Tech

**Programming:** Python · TypeScript / JavaScript · Java · C++ · SQL
**AI / ML & data:** scikit-learn · XGBoost · NetworkX · pandas · NumPy · statsmodels · matplotlib
**Backend & web:** FastAPI · Node.js · PostgreSQL · Docker · React · Next.js
**Tools:** Git · LaTeX

---

📫 **pedromoreiracg@gmail.com** · [LinkedIn](https://linkedin.com/in/pedro-henrique-334984263)
