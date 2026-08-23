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

**[Concepts2Metrics](https://github.com/Igluminati/Concepts2Metrics)**

Built during a data science internship at Zappi in London: a Python pipeline
using XGBoost and SHAP to identify which features of a product concept
actually move outcome metrics.

## Not yet public

These are finished and I am happy to walk through the code or the write-up on
request. They are private for now while the write-ups are still in progress.

**Recursive leverage in yield-bearing stablecoins.** MSc project with the UZH
Blockchain and Distributed Ledger group (Prof. Claudio Tessone, Krzysztof
Gogol). A daily on-chain panel of 23 large leveraged "loopers" on Aave v3 and
Morpho Blue: HDBSCAN/UMAP to separate behavioural cohorts, then XGBoost with
SHAP attribution to explain which positions unwind under stress rather than
only predicting that they will. ROC-AUC 0.90 and 0.98 on the two
classification tasks.

**Multi-token DeFi staking pool on Base.** Team project for the Seminar in
Blockchain Programming at UZH, graded 5.5/6. A pool accepting WETH, USDC and
EURC that forwards deposits into Morpho MetaMorpho vaults, with
harvestable-yield accounting and a 24-hour Chainlink Automation job driving
the harvest cycle. Solidity, Hardhat, Chainlink.

**Visual odometry from a phone camera.** Monocular VO (FAST, KLT, PnP RANSAC)
with 100% pose success across 13,000+ frames, then fused Samsung S20 IMU and
gyro data from a Swiss cablecar recording to recover metric scale (4.2x) and
match barometric elevation to within 1.2%.

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

*Languages: English (native), Albanian (fluent), German (A1.2, in progress).*
