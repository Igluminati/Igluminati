# Igli Kristo

MSc Informatics at the University of Zurich. Artificial Intelligence major,
Data Science minor. Based in Luzern, Switzerland.

I work on making model outputs checkable: whether an answer can be traced to a
source, and whether a system fails evenly across the people it is used on.
Before Zurich I did a BSc in Computer Science at Royal Holloway, University of
London.

**Currently looking for** a working-student or research-assistant role in
Switzerland, 15 h/week during term and full-time in the lecture-free period.
Graduating July 2027.

## Selected work

**[ai-authorship-detection](https://github.com/Igluminati/ai-authorship-detection)**

Detecting machine-generated academic essays with a multi-view ensemble
(DeBERTa-v3, RoBERTa likelihood features, stylometry). The interesting result
is not the F1 score. The evaluation asks whether false positives land
disproportionately on non-native English writers, because a detector with
strong headline accuracy can still be unusable for anyone writing in a second
language. Four-person team; I built the preprocessing and tokenisation over an
800k-sample corpus and the non-native hold-out set.

**Visual odometry from a phone camera**
· [full report (PDF)](https://iglikristo.xyz/vamr-miniproj.pdf)

Monocular VO (FAST, KLT, PnP RANSAC) with 100% pose success across 13,000+
frames. A single camera recovers its path but not its scale, and a fast
rotation is enough to lose the track, so we filmed a Swiss cablecar on a
Samsung S20 and used the phone's gyroscope to survive the rotations and its
IMU to put the trajectory into metres: 4.2x scale recovery, matching
barometric elevation to within 1.2%.

**Knowledge-graph QA chatbot**
· [report (PDF)](https://iglikristo.xyz/atai-bot-report.pdf)

Answers questions from a Wikidata-derived knowledge graph. SPARQL first,
embeddings when the graph has no hit, and only then a local LLM on Ollama, so
that an answer points at a source instead of being generated freely.

**Recursive leverage in yield-bearing stablecoins**
· [overview](https://iglikristo.xyz)

MSc project with Dawid Rymarczyk, supervised by Prof. Claudio Tessone and
Krzysztof Gogol at UZH. Large wallets loop yield-bearing stablecoins on Aave
v3 and Morpho Blue to stack extra yield. We ask whether they are really
following a handful of shared strategies, how those strategies differ in risk
management, and whether the on-chain state of a position can tell you a
stressful day is coming. HDBSCAN/UMAP for the cohorts, XGBoost with SHAP
attribution for the prediction, ROC-AUC 0.90 and 0.98. Code private until the
write-up is submitted.

**Multi-token DeFi staking pool on Base**
· [overview](https://iglikristo.xyz)

Most staking apps pay you by printing a new token. This one does not: you
deposit WETH, USDC or EURC, the contract routes it into a Morpho MetaMorpho
vault, and a daily Chainlink Automation harvest returns the yield in the same
token you put in. Team project for the Seminar in Blockchain Programming at
UZH, graded 5.5/6.

**[Concepts2Metrics](https://github.com/Igluminati/Concepts2Metrics)**

Built during a data science internship at Zappi in London: a Python pipeline
using XGBoost and SHAP to identify which features of a product concept
actually move outcome metrics.

## Stack

- **Languages:** Python · Java · TypeScript/JavaScript · Solidity · SQL · C++ · Bash · LaTeX
- **ML:** PyTorch · scikit-learn · XGBoost · SHAP · HDBSCAN/UMAP · SpaCy · transformers · Ollama
- **Data and web:** pandas · NumPy · Jupyter · Next.js · React · Prisma · tRPC · MySQL
- **Vision:** OpenCV · visual odometry · camera and IMU sensor fusion
- **Chain:** Hardhat · ethers.js · OpenZeppelin · Chainlink · Gnosis Safe
- **Tools:** Git · Linux (Arch/Manjaro, Debian) · Docker · Vim

## Elsewhere

[iglikristo.xyz](https://iglikristo.xyz) ·
[LinkedIn](https://www.linkedin.com/in/igli-k-652b66189/) ·
igli.kristo@uzh.ch

*Languages: English (native), Albanian (fluent), German (A1.2, continuing each
semester at the UZH Language Center; A2.2 expected by graduation).*
