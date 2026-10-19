# Igli Kristo

MSc Informatics at the University of Zurich (AI major, Data Science minor).
BSc Computer Science at Royal Holloway. Based in Luzern.

Most of the work is Python and Jupyter, plus Solidity when it's on-chain.
Since June 2025 I've been writing Solidity at FVC Asset Group, remote from
Luzern. Token, sale and vesting are on Ethereum mainnet, with a tested
staking contract, Chainlink pricing, and a Gnosis Safe treasury:
[FVCDigital/fvc](https://github.com/FVCDigital/fvc). This semester I'm a
teaching assistant for Essentials in Text and Speech Processing at UZH.

## Projects

### [Recursive leverage in yield-bearing stablecoins](https://github.com/Igluminati/recursive-leverage-defi)

[Report (PDF)](https://github.com/Igluminati/recursive-leverage-defi/blob/main/paper/Recursive_Leverage_in_Yield_Bearing_Stablecoins__Proof_of_Concept_and_Empirical_Analysis.pdf)

MSc project with Dawid Rymarczyk, supervised by Claudio Tessone and
Krzysztof Gogol.

Large wallets on Aave v3 and Morpho Blue borrow against yield-bearing
stablecoins and deposit the proceeds again, to stack the yield. We followed
the 23 largest positions day by day. HDBSCAN found three behaviours: holding at
low leverage, looping actively, and sitting at max leverage near liquidation.
The first clustering mostly grouped days from the same wallet. I fixed that
before we treated the groups as strategies.

XGBoost and SHAP for two labels: a stressed day, and a cut in risk. The
stressed-day model came back at ROC-AUC 1.00, which was target leakage.
Without it: 0.98 on stressed days, 0.90 on rebalancing. No liquidations in
the sample. A 3-5% price fall would still raise liquidatable Aave collateral
from about $40M to over $510M. I wrote the Aave pipeline and its tests.

### [Visual odometry from a phone camera](https://github.com/SubOptimal-Controllers/VizOdometryPipeline)

[Report (PDF)](https://iglikristo.xyz/vamr-miniproj.pdf)

VAMR mini-project. Monocular VO with FAST, KLT and PnP RANSAC. Pose
estimation held across 13,000+ frames.

A single camera recovers the path but not the scale, and a fast rotation
loses the track. We filmed a Swiss cablecar on a Samsung S20, used the
gyroscope through the rotations, and the IMU to put the trajectory in metres.
Scale came out 4.2x. Elevation matched the barometer within 1.2%.

### [ai-authorship-detection](https://github.com/Igluminati/ai-authorship-detection)

Four of us, for the same text-and-speech course. A detector for
machine-written academic essays: DeBERTa-v3, RoBERTa likelihood features,
stylometry. I did the preprocessing and tokenisation on an 800k-sample
corpus, and built a hold-out of non-native English essays. We reported
macro-F1 and the false-positive rate on that hold-out.

### Staking pool on Base

Seminar in Blockchain Programming at UZH, graded 5.5/6.
[Notes](https://iglikristo.xyz).

Deposit WETH, USDC or EURC. The contract sends it to a Morpho MetaMorpho
vault. Once a day, Chainlink Automation harvests and pays the yield in the
token that was deposited.

### [Knowledge-graph QA chatbot](https://iglikristo.xyz/atai-bot-report.pdf)

Questions over a Wikidata graph. SPARQL first, embeddings when the graph has
no hit, then a local model on Ollama. It ran on Speakeasy, with the queries
logged.

### [Concepts2Metrics](https://github.com/Igluminati/Concepts2Metrics)

Internship at Zappi in London, August to September 2023, with Kristupas
Jucaitis. XGBoost and SHAP on product-concept tags. Train RMSE down 15%,
test RMSE down 10%.

## Tools

Python, SQL, Java, TypeScript, Solidity, C++.
PyTorch, scikit-learn, XGBoost, SHAP, HDBSCAN, transformers, SpaCy, OpenCV.
Next.js, React, Prisma, tRPC, Hardhat, ethers.js, Chainlink, Gnosis Safe.

[iglikristo.xyz](https://iglikristo.xyz) ·
[LinkedIn](https://www.linkedin.com/in/igli-k-652b66189/) ·
[igli.kristo@uzh.ch](mailto:igli.kristo@uzh.ch) ·
[IgliKristo@protonmail.com](mailto:IgliKristo@protonmail.com)

English (native), Albanian (fluent), German (A1.2).
