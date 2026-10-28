# My AI Engineering Path
<!-- Managed by the ai-engineering-from-scratch learning skills.
     Repo: https://github.com/rohitg00/ai-engineering-from-scratch -->

## Mission
Career change into AI/ML engineering. I self-study each section from the GitHub repo, then get quizzed (10 questions per section). Score > 5/10 → section marked Done. After completing all sections in a phase, I receive a phase-end project to build and push to GitHub. The tutor reviews my code quality and output, gives feedback, and logs it here.

## Tutor & AI Agent Operating Guidelines

> **Note for any AI Agent / Tutor:** When reviewing, resuming, or running this study curriculum in any environment or IDE, you must strictly adhere to the following protocol for quiz generation, grading, feedback, and tracking updates.

### 1. Curriculum Source & Content Ingestion
- **Official Repository:** `https://github.com/rohitg00/ai-engineering-from-scratch`
- **Documentation Path:** `phases/<phase-folder>/<lesson-folder>/docs/en.md` (or raw markdown from `https://raw.githubusercontent.com/rohitg00/ai-engineering-from-scratch/main/...`)
- Before quizzing the learner on any section, retrieve the full lesson document (or code files) to ground all questions directly in the official curriculum material.

### 2. Quiz Format & Delivery Specification
- **Question Count:** Exactly **10 questions** per section/lesson.
- **Option Structure:** Multiple-choice with exactly **4 options** per question.
- **Single-Select Only:** Exactly one correct option per question (`is_multi_select: false`). Do not use "All of the above", "None of the above", or "Select all that apply".
- **Strict Option Length Limit (Max 2 Lines):** Every option must be concise and capped at a maximum of **2 lines**. All 4 options must have balanced length and technical detail. NEVER make the correct option longer or more detailed than the distractors.
- **Randomized Correct Option Positioning:** The correct answer **MUST be randomly and evenly distributed** across positions (A, B, C, D) throughout the 10 questions (~2-3 of each). Never bias or default toward Option A as the correct answer.
- **Delivery Mode:** 
  - If using an interactive UI/modal tool (e.g., `ask_question`), emit all 10 questions in a single interactive prompt with options formatted as clean, direct statements (framed as the user's response).
  - If in standard chat/CLI without interactive tool support, present the 10 questions clearly numbered Q1–Q10 with lettered options (A, B, C, D) and await user responses.

### 3. Difficulty Level & Question Design Criteria
- **Rigorous, Concept-Driven, and Production-Relevant:** Questions must NOT be trivial vocabulary checks, superficial recall, or pure syntax memorization. Frame them at the caliber of recruiting/interviewing Senior AI/ML Engineers at top AI MNCs (OpenAI, DeepMind, Anthropic, Meta FAIR).
- **Target Difficulty:** Advanced undergraduate to applied industry level (AI/ML Engineering).
- **Core Focus Areas:**
  - **Mathematical & Geometric Intuition:** (e.g., SVD geometric sequence: $V^T$ rotate $\to$ $\Sigma$ scale $\to$ $U$ rotate; Laplacian eigenvalues; Hermitian/conjugate symmetries in frequency domain; positive semi-definiteness).
  - **Algorithmic Mechanics & Complexity:** Direct computation vs. fast algorithms (e.g., direct DFT $O(N^2)$ vs. FFT $O(N \log N)$), divide-and-conquer steps, recursion, convergence conditions.
  - **Applied ML / Deep Learning Connections:** How mathematical theory maps to neural architectures (e.g., GCN self-loops $\hat{A} = A + I$, convolution theorem in CNNs, spectral clustering via Fiedler vector, Adam/Momentum hyperparameters, float32 numerical overflow).
  - **Symmetric High-Quality Distractors:** Distractors must be realistic engineering and mathematical misconceptions matching the exact length, vocabulary, and technical sophistication of the correct answer, preventing elimination by superficial cues.

### 4. Grading Criteria & Scoring Thresholds
- **Passing Threshold:** **> 5 / 10** (i.e. $\ge 6/10$).
  - Score $\ge 6/10 \implies$ Marked as **✅ Done / Pass**.
  - Score $\le 5/10 \implies$ Marked as **🔁 Retry** (and added to the `## Review Queue` table for future re-testing).

### 5. Post-Quiz Feedback & Review Schema
After the learner submits their answers, the tutor must immediately output:
1. **Header & Overall Score:** e.g., `### Quiz Results: Phase X — Section Y: <Name>` followed by `**Score: X / 10** (Pass ✅ or Retry 🔁)`.
2. **Detailed Review of Missed Questions:** For every missed question:
   - **Question:** Full question text.
   - **Your Answer:** The learner's submitted option.
   - **Correct Answer:** The correct option.
   - **Explanation:** In-depth explanation analyzing the underlying mathematics/concept, clarifying *why* the correct answer holds and *why* the learner's choice was mistaken.
3. **Phase Progress Summary & Remaining Roadmap:** A concise table of remaining sections in the current phase prompting for the next section.

### 6. Strict Protocol for Updating `LEARNING.md`
Whenever a quiz is completed, the tutor must automatically make the following 3 updates to this file:
1. **Phase Header Status Count:** Increment the completed section count (e.g., `> GitHub: phases/01_Math_Foundations/ | Status: 🔄 In Progress (20/22 done)`).
2. **Phase Table Row:** Locate the section row and update its score and badge:
   `| <Num> | <Section Name> | <Score>/10 | ✅ |`
3. **Progress Log Entry:** Append a new row to the `## Progress Log` table at the bottom:
   `| YYYY-MM-DD | Phase <N> | <Num> — <Section Name> | <Score>/10 | ✅ Pass | <Detailed summary of score, key concepts mastered, and exact missed questions/misconceptions> |`

### 7. Phase Projects & Unlocking
- Once all sections in a phase are marked ✅ Done, the Phase-End Project unlocks.
- The tutor assigns the project requirements based on the phase curriculum.
- The learner completes the project in a GitHub repository and provides the repo link.
- The tutor reviews the project code quality, CLI/notebook implementation, tests, error handling, Docker/uv configuration, and output.
- The tutor evaluates, assigns a grade (e.g. A+), and records the entry under `## Phase Projects Log`.

## Placement
- Date: 2026-08-22
- Score: 8/10 (Math & Stats: 2/2 | Classical ML: 1/2 | Deep Learning: 1/2 | NLP & Transformers: 2/2 | Applied AI: 2/2)
- Decision: Revising everything from Phase 0 (full curriculum run)
- Pace: ~5 hours/week

## Path
| Phase | Name                          | Lessons | Status      | Est. Hours |
|-------|-------------------------------|---------|-------------|------------|
| 0     | Setup & Tooling               | 12      | ✅ Done        | 14      |
| 1     | Math Foundations              | 22      | 🔄 Ready for Project (22/22) | 23      |
| 2     | ML Fundamentals               | 18      | 🔲 Not Started | 21      |
| 3     | Deep Learning Core            | 13      | 🔲 Not Started | 15      |
| 4     | Computer Vision               | 28      | 🔲 Not Started | 27      |
| 5     | NLP — Foundations to Advanced | 29      | 🔲 Not Started | 30      |
| 6     | Speech & Audio                | 17      | 🔲 Not Started | 18      |
| 7     | Transformers Deep Dive        | 16      | 🔲 Not Started | 14      |
| 8     | Generative AI                 | ~15     | 🔲 Not Started | 14      |
| 9     | LLM Pre-Training              | ~15     | 🔲 Not Started | ~18     |
| 10    | LLM Fine-Tuning & Alignment   | ~15     | 🔲 Not Started | ~18     |
| 11    | LLM Engineering               | ~15     | 🔲 Not Started | ~20     |
| 12    | RAG & Knowledge Systems       | ~15     | 🔲 Not Started | ~20     |
| 13    | AI Products & Deployment      | ~15     | 🔲 Not Started | ~18     |
| 14    | Agent Engineering             | ~15     | 🔲 Not Started | ~22     |
| 15    | Multi-Agent Systems           | ~15     | 🔲 Not Started | ~18     |
| 16    | AI Infrastructure & MLOps     | ~15     | 🔲 Not Started | ~20     |
| 17    | Multimodal AI                 | ~15     | 🔲 Not Started | ~18     |
| 18    | AI Safety & Alignment         | ~15     | 🔲 Not Started | ~15     |
| 19    | Capstone & Portfolio          | ~10     | 🔲 Not Started | ~20     |

> **Total:** ~314 hours across 20 phases | At 5h/week ≈ 63 weeks

---

## Phase 0 — Setup & Tooling
> GitHub: `phases/00_Setup_AI/` | Status: ✅ Done (12/12)

| # | Section / Lesson | Quiz Score | Status |
|---|-----------------|------------|--------|
| 01 | Dev Environment | 10/10 | ✅ |
| 02 | Git & Collaboration | 9/10 | ✅ |
| 03 | GPU Setup & Cloud | 10/10 | ✅ |
| 04 | APIs & Keys | 10/10 | ✅ |
| 05 | Jupyter Notebooks | 10/10 | ✅ |
| 06 | Python Environments | 8/10 | ✅ |
| 07 | Docker for AI | 8/10 | ✅ |
| 08 | Editor Setup | 8/10 | ✅ |
| 09 | Data Management | 5/10 | ✅ |
| 10 | Terminal & Shell | 6/10 | ✅ |
| 11 | Linux for AI | 6/10 | ✅ |
| 12 | Debugging & Profiling | 6/10 | ✅ |

**Phase 0 Project:** ✅ Passed & Evaluated
**Project Result:** Grade: A+ | Repo: [preetshah0/phase0-ai-dev-environment](https://github.com/preetshah0/phase0-ai-dev-environment)

---

## Phase 1 — Math Foundations
> GitHub: `phases/01_Math_Foundations/` | Status: 🔄 Ready for Phase Project (22/22 done)

| # | Section / Lesson | Quiz Score | Status |
|---|-----------------|------------|--------|
| 01 | Linear Algebra Intuition | 9/10 | ✅ |
| 02 | Vectors, Matrices & Operations | 10/10 | ✅ |
| 03 | Matrix Transformations & Eigenvalues | 8/10 | ✅ |
| 04 | Calculus for ML — Derivatives & Gradients | 7/10 | ✅ |
| 05 | Chain Rule & Automatic Differentiation | 7/10 | ✅ |
| 06 | Probability & Distributions | 8/10 | ✅ |
| 07 | Bayes' Theorem & Statistical Thinking | 10/10 | ✅ |
| 08 | Optimization — Gradient Descent Family | 7/10 | ✅ |
| 09 | Information Theory — Entropy, KL Divergence | 7/10 | ✅ |
| 10 | Dimensionality Reduction — PCA, t-SNE, UMAP | 6/10 | ✅ |
| 11 | Singular Value Decomposition | 7/10 | ✅ |
| 12 | Tensor Operations | 8/10 | ✅ |
| 13 | Numerical Stability | 9/10 | ✅ |
| 14 | Norms & Distances | 9/10 | ✅ |
| 15 | Statistics for ML | 9/10 | ✅ |
| 16 | Sampling Methods | 7/10 | ✅ |
| 17 | Linear Systems | 8/10 | ✅ |
| 18 | Convex Optimization | 9/10 | ✅ |
| 19 | Complex Numbers for AI | 9/10 | ✅ |
| 20 | The Fourier Transform | 9/10 | ✅ |
| 21 | Graph Theory for ML | 10/10 | ✅ |
| 22 | Stochastic Processes | 9/10 | ✅ |

**Phase 1 Project:** 🔓 Unlocked (All 22 sections Completed)
**Project Result:** In Progress

---

## Phase 2 — ML Fundamentals
> Status: 🔒 Locked

| # | Section / Lesson | Quiz Score | Status |
|---|-----------------|------------|--------|
| 01 | What Is Machine Learning — Types & Taxonomy | --/10 | 🔲 |
| 02 | Linear Regression from Scratch | --/10 | 🔲 |
| 03 | Logistic Regression & Classification | --/10 | 🔲 |
| 04 | Decision Trees & Random Forests | --/10 | 🔲 |
| 05 | Support Vector Machines | --/10 | 🔲 |
| 06 | K-Nearest Neighbors & Distance Metrics | --/10 | 🔲 |
| 07 | Unsupervised Learning — K-Means, DBSCAN | --/10 | 🔲 |
| 08 | Feature Engineering & Selection | --/10 | 🔲 |
| 09 | Model Evaluation — Metrics, Cross-Validation | --/10 | 🔲 |
| 10 | Bias, Variance & the Learning Curve | --/10 | 🔲 |
| 11 | Ensemble Methods — Boosting, Bagging, Stacking | --/10 | 🔲 |
| 12 | Hyperparameter Tuning & AutoML | --/10 | 🔲 |
| 13 | ML Pipelines & Experiment Tracking | --/10 | 🔲 |
| 14 | Naive Bayes — Multinomial, Gaussian, Bernoulli | --/10 | 🔲 |
| 15 | Time Series Fundamentals | --/10 | 🔲 |
| 16 | Anomaly Detection | --/10 | 🔲 |
| 17 | Handling Imbalanced Data | --/10 | 🔲 |
| 18 | Feature Selection | --/10 | 🔲 |

**Phase 2 Project:** 🔒 Unlocks when all 18 sections are Done
**Project Result:** --

---

## Progress Log
| Date | Phase | Section | Score | Status | Note |
| 2026-08-22 | Phase 0 | 01 — Dev Environment | 10/10 | ✅ Pass | Perfect score — strong grasp of venvs, pip/conda, uv, Docker, secrets management |
| 2026-08-23 | Phase 0 | 11 — Linux for AI | 6/10 | ✅ Pass | Missed: chmod 755 notation, ps aux pipe, grep -r vs find |
| 2026-08-23 | Phase 0 | 12 — Debugging & Profiling | 6/10 | ✅ Pass | Missed: pdb import syntax, cProfile flag, traceback direction, memory_profiler vs cProfile |
| 2026-08-23 | Phase 0 | 02 — Git & Collaboration | 9/10 | ✅ Pass | Missed: git reset HEAD~1 vs git revert distinction |
| 2026-08-23 | Phase 0 | 03 — GPU Setup & Cloud | 10/10 | ✅ Pass | Perfect score |
| 2026-08-23 | Phase 0 | 04 — APIs & Keys | 10/10 | ✅ Pass | Perfect score |
| 2026-08-23 | Phase 0 | 05 — Jupyter Notebooks | 10/10 | ✅ Pass | Perfect score |
| 2026-08-23 | Phase 0 | 06 — Python Environments | 8/10 | ✅ Pass | Missed: venv recreation vs pip fix, sys.prefix vs VIRTUAL_ENV |
| 2026-08-23 | Phase 0 | 07 — Docker for AI | 8/10 | ✅ Pass | Missed: container vs VM (shared kernel), ARG vs ENV direction |
| 2026-08-23 | Phase 0 | 08 — Editor Setup | 8/10 | ✅ Pass | Missed: Black formatter key (deprecated), Ctrl+Shift+G for Git |
| 2026-08-23 | Phase 0 | 09 — Data Management | 5/10 | ✅ Pass | Missed: df.info vs describe, interpolate for time-series, Parquet, raw text storage, stratify= |
| 2026-08-23 | Phase 0 | 10 — Terminal & Shell | 6/10 | ✅ Pass | Missed: pipe vs &&, find -mtime, history grep, &> for stderr |
| 2026-08-25 | Phase 1 | 01 — Linear Algebra Intuition | 9/10 | ✅ Pass | Excellent! Missed: rank definition (linearly independent cols/rows) |
| 2026-08-27 | Phase 1 | 02 — Vectors, Matrices & Operations | 10/10 | ✅ Pass | Perfect score — mastered inner dimensions, Hadamard vs matrix multiplication, broadcasting, weight shapes, transpose |
| 2026-08-27 | Phase 1 | 03 — Matrix Transformations & Eigenvalues | 8/10 | ✅ Pass | Excellent! Missed: horizontal shear matrix Shx vs Shy, composition order notation B@A@v |
| 2026-08-28 | Phase 1 | 04 — Calculus for ML — Derivatives & Gradients | 7/10 | ✅ Pass | Pass! Missed: gradient vector direction (steepest ascent), chain rule formula, positive definite Hessian (local minimum) |
| 2026-09-01 | Phase 1 | 05 — Chain Rule & Automatic Differentiation | 7/10 | ✅ Pass | Pass! Missed: dual numbers property (ε^2=0 vs i^2=-1), PyTorch grad accumulation (D), addition node grad pass (A) |
| 2026-09-01 | Phase 1 | 06 — Probability & Distributions | 8/10 | ✅ Pass | Excellent! Missed: independent joint prob multiplication P(A)*P(B), Poisson variance (λ) |
| 2026-09-10 | Phase 1 | 09 — Information Theory — Entropy, KL Divergence | 7/10 | ✅ Pass | Pass! Missed: fair coin entropy (1.00 bit vs 0.08 bit), classification cross-entropy simplification (-log(q(true_class))), conditional entropy when X determines Y (0) |
| 2026-09-12 | Phase 1 | 10 — Dimensionality Reduction — PCA, t-SNE, UMAP | 6/10 | ✅ Pass | Pass! Missed: distance ratio convergence (~1.0), hypercube corners (2^d), covariance matrix property (symmetric & positive semi-definite), UMAP n_neighbors effect (global structure) |
| 2026-09-12 | Phase 1 | 12 — Tensor Operations | 8/10 | ✅ Pass | Excellent! Missed: PyTorch image layout (NCHW vs NHWC), einsum matrix trace notation (ii-> vs i,j->ij) |
| 2026-09-12 | Phase 1 | 08 — Optimization — Gradient Descent Family | 7/10 | ✅ Pass | Pass! Missed: mini-batch stochastic noise benefit (escape local minima/saddle points vs exact gradient), momentum beta default (0.9 vs 0.001), Adam default hyperparameters (lr=0.001, beta1=0.9, beta2=0.999, eps=1e-8) |
| 2026-09-12 | Phase 1 | 13 — Numerical Stability | 9/10 | ✅ Pass | Exceptional! Missed: exp(x) float32 overflow threshold (x > 89.0 vs x > 1.0) |
| 2026-09-27 | Phase 1 | 14 — Norms & Distances | 9/10 | ✅ Pass | Exceptional! Missed: Mahalanobis distance when covariance is identity matrix (simplifies to Euclidean distance L2 vs Cosine distance) |
| 2026-09-27 | Phase 1 | 15 — Statistics for ML | 9/10 | ✅ Pass | Exceptional! Missed: monotonic non-linear correlation (Pearson r < 1.0, Spearman rho = 1.0 vs Pearson r = 1.0, Spearman rho < 1.0) |
| 2026-10-11 | Phase 1 | 16 — Sampling Methods | 7/10 | ✅ Pass | Pass! Missed: exponential inverse CDF formula (-ln(u)/lambda vs lambda*exp(-u)), Metropolis-Hastings stationary distribution condition (Detailed Balance vs Central Limit Theorem), Gibbs sampling acceptance rate (100% / 1.0 vs ~0.234) |
| 2026-10-11 | Phase 1 | 18 — Convex Optimization | 9/10 | ✅ Pass | Exceptional! Missed: formal definition of convex set (line segment tx + (1-t)y in S vs set of positive real numbers) |
| 2026-10-11 | Phase 1 | 07 — Bayes' Theorem & Statistical Thinking | 10/10 | ✅ Pass | Perfect score — mastered Bayes' rule components, rare disease prior dominance, Naive Bayes independence assumption & numerator ranking, Laplace smoothing, MLE vs MAP & regularization connection, Bayesian vs Frequentist paradigms |
| 2026-10-13 | Phase 1 | 19 — Complex Numbers for AI | 9/10 | ✅ Pass | Exceptional! Missed: polar form multiplication rule (magnitudes multiply, angles add — not magnitudes add, angles multiply) |
| 2026-10-13 | Phase 1 | 11 — Singular Value Decomposition | 7/10 | ✅ Pass | Pass! Missed: SVD geometric sequence (Rotate→Scale→Rotate vs Scale→Rotate→Scale), outer product form (sum of rank-1 outer products vs det(Σ)·U·Vᵀ), AᵀA relationship (V are eigenvectors of AᵀA not AAᵀ; σᵢ² are eigenvalues not σᵢ) |
| 2026-10-15 | Phase 1 | 20 — The Fourier Transform | 9/10 | ✅ Pass | Exceptional! Missed: real-valued signal DFT symmetry (X[N-k] = conjugate(X[k]) Hermitian symmetry vs X[N-k] = X[k]) |
| 2026-10-15 | Phase 1 | 21 — Graph Theory for ML | 10/10 | ✅ Pass | Perfect score — mastered adjacency & degree matrices, BFS vs DFS properties, graph Laplacian L = D - A positive semi-definiteness & zero eigenvalues (connected components), Fiedler value & spectral clustering, K-hop GNN message passing, and GCN self-loops (Â = A + I) |
| 2026-10-25 | Phase 1 | 22 — Stochastic Processes | 9/10 | ✅ Pass | Exceptional! Missed: spectral gap vs mixing time (larger spectral gap implies faster mixing / shorter mixing time t_mix ~ 1/spectral_gap) |
| 2026-10-25 | Phase 1 | 17 — Linear Systems | 8/10 | ✅ Pass | Pass! Advanced MNC level. Missed: relative error bound via condition number kappa(A) not det(A) (||Δx||/||x|| <= kappa(A) ||Δb||/||b||), underdetermined minimum-norm solution uses right pseudoinverse x* = Aᵀ(A Aᵀ)⁻¹b (AᵀA is singular for m < n) |
|------|-------|---------|-------|--------|------|

---

## Phase Projects Log
| Date | Phase | Project | Repo/Folder | Code Quality | Output | Grade | Feedback |
| 2026-08-23 | Phase 0 | AI Dev Environment | [GitHub](https://github.com/preetshah0/phase0-ai-dev-environment) / `phase0-ai-dev-enviornment` | Excellent (A+) | Verified (Exit Code 1 on warning threshold) | A+ | Exemplary project structure with `uv`, multi-stage Dockerfile, robust CLI `data_check.py` with logging & argparse, complete EDA notebook, and zero committed secrets. |
|------|-------|---------|-------------|--------------|--------|-------|----------|

---

## Review Queue
<!-- Sections scoring ≤ 5/10 are added here for retry -->

