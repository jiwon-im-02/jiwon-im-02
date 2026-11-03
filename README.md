### 👋 Hello! I'm Jiwon Im (임지원)

I'm an M.S. student in **Statistics & Data Science** at **Chungnam National University** (High-Dimensional Data Analysis Lab), graduating Feb. 2027.
My research is on **graph neural networks**, **statistical learning**, and **interpretable predictive modeling** for high-dimensional and spatio-temporal data, from Hi-C genomic contact matrices to skeleton-based video.
I care about data quality and reproducibility: I work out where a model or a decision criterion breaks before I trust it.

<p>
  <a href="mailto:jiwonlim0492@gmail.com"><img src="https://img.shields.io/badge/Email-jiwonlim0492%40gmail.com-EA4335?style=flat-square&logo=gmail&logoColor=white" alt="Email"/></a>
  <a href="https://wony-wony.tistory.com"><img src="https://img.shields.io/badge/Blog-wony--wony.tistory.com-000000?style=flat-square&logo=tistory&logoColor=white" alt="Blog"/></a>
</p>

* * *

### 🔍 Research Interests

*   🧬 **Graph Neural Networks for high-dimensional data**: sparse graph construction, Hi-C / genomic data
*   🎥 **Robust spatio-temporal modeling**: skeleton-based action recognition, low-light robustness, anomaly detection
*   📊 **Statistical learning & validation**: interpretable prediction, mixed models, survival analysis, reproducibility and agreement analysis

* * *

### 📄 Publications

*   **Sparse Weighted Graph Convolutional Networks for Colorectal Cancer Classification Using Hi-C Data**  
    Mingyu Go, **Jiwon Im**, Insu Jang, Minsu Park — *Scientific Reports* (2026)
*   **Robust Physical Distress Detection in Low-Light Environments via Spatio-Temporal Graph Convolutional Networks**  
    **Jiwon Im**, Yunchae Jung, Minsu Park — *PLOS ONE* (in preparation)

<details>
<summary><b>🎤 Conference Presentations (8)</b></summary>

*   **Robust Skeleton-Based Physical Distress Detection via Illumination-Aware Graph Convolutional Networks**: ISCB-GMDS 2026, Freiburg, Germany (Sep. 2026), Poster
*   **Robust Spatio-Temporal Graph Modeling for Behavior Monitoring under Heterogeneous Environments**: EcoSta 2026, Kyoto, Japan (Aug. 2026), Poster
*   **저조도 환경 내 이상행동 탐지 안정화 기법: 조도 적응형 시공간 그래프 임베딩**: 한국품질경영학회 춘계학술대회 (2026.05), 🏆 우수발표논문상
*   **Robust Physical Distress Detection in Low-Light Environments via ST-GCN**: 한국데이터정보과학회 춘계학술대회 (2026.05), 🏆 논문발표상 장려상
*   **무인점포 안전관리를 위한 Skeleton-Context 기반 실시간 이상행동 탐지 모델**: 한국자료분석학회 동계학술대회 (2025.11), 구두 발표, 🏆 장려상 (구두논문 부문)
*   **Wavelet Scattering Meet Transformers: Detecting Anomalies in Robotic Trajectories** (공동저자): 한국자료분석학회 동계학술대회 (2025.11), 포스터, 🏆 장려상 (포스터논문 부문)
*   **Integrating High-Dimensional Hi-C Data with Sparse Graph Neural Networks for Enhanced Colorectal Cancer Prediction**: ISCB 2025, Basel, Switzerland (Aug. 2025), Poster
*   **Sparse Graph Neural Networks for High-dimensional Genomic Data Integration**: 한국통계학회 하계학술대회 (2025.06), 포스터

</details>

* * *

### 🚀 Projects

*   **🧬 Sparse Weighted GCN for Hi-C Colorectal Cancer Classification** (2024 – 2025)  
    Hi-C contact matrices are noisy, so a plain GCN also learns the noise. Kept only informative contacts via bi-square kernel weights with adaptive bandwidth, evaluated with nested 10-fold CV on 102 subjects, and compared against GCN, CNN, GraphSAGE and GAT.  
    → **92.2% accuracy** (bootstrap 95% CI 87.3–97.1%), F1 94.4%, ~36% less training time. `PyTorch` `GNN` `Hi-C`

*   **🌙 Low-Light Robust Skeleton-Based Distress Detection** (2025 – present, M.S. research)  
    Skeleton graph (CTR-GCN and other GCN backbones) fused with CNN scene context, trained with illumination-aware augmentation. Built ~114K clips from NTU RGB+D and synthetic Mild/Moderate/Extreme low-light versions, filtering failed or low-confidence pose extractions.  
    → **+4.1%p accuracy** in the darkest condition with only 1.51% extra parameters, ~0.30 ms inference. `PyTorch` `YOLOv8-Pose` `ST-GCN` `CTR-GCN`

*   **🏪 OneWay Guard: Real-Time Abnormal Behavior Detection for Unmanned Stores** (2025, team lead)  
    End-to-end prototype: YOLOv8-Pose 17-joint sequences + ResNet scene features → CTR-GCN classifier → TorchScript export → React (Vite) PWA real-time monitoring dashboard. Joint-confidence thresholds set from normal-condition data distributions, with Kalman filter smoothing.  
    → 🏆 **우수상**, 충남대 Data Science Challenge (28개 팀). `PyTorch` `TorchScript` `React` `PWA`

*   **🤖 Wavelet Scattering + Transformer for Robotic Trajectory Anomaly Detection** (2025, co-author)  
    Unsupervised anomaly detection on multivariate sensor time series trained on normal patterns only: wavelet scattering features that are robust to time shifts, plus a Transformer encoder for temporal dependencies. Catches subtle vibration bursts and frequency drift. `Time Series` `Transformer`

*   **🚛 ROUTE:ONE: Empty-Trip-Aware Container Truck Dispatch Recommender** (2026 K-DATA SCIENCE 해커톤)  
    On 16K container-transport records (3 months), a rule-based module first identifies empty-trip segments (recall 95.9%, precision 88.6%). A LightGBM model with 30 features then predicts when a subcontracted truck will be needed, validated on a time-based split (Jan–Feb train / Mar test), and a scoring engine recommends company-owned trucks for each new order. Served as a Flask web app with map-based route comparison and dispatch confirmation.  
    → ROC-AUC **0.845** (beats logistic regression and rule baselines); 🏆 **창의상** (본선 26개 팀). `LightGBM` `Flask` `Logistics`

*   **✍️ AI Handwritten Signature Verification** (2025 K-DATA SCIENCE 해커톤)  
    Dual verification: a Siamese CNN for image similarity and an RNN for behavioral time series (speed, pressure, trajectory), run independently to reduce both false accepts and false rejects.  
    → 🏆 **창의상** (본선 26개 팀). `CNN` `RNN` `Siamese Network`

*   **💬 Network-Based Emotion Analysis for Social Isolation** (2024 K-DATA SCIENCE 해커톤)  
    SBERT embeddings of ~1,200 AI Hub emotional dialogues → PCA (768→50) → soft-cosine similarity graph → GraphSAGE emotion classification.  
    → 🏆 **창의상** (본선 26개 팀). `NLP` `SBERT` `GraphSAGE`

*   **🗺️ Spatial Analysis of Vacant Houses and Crime in Busan** (2024 통계데이터활용대회)  
    GIS + geographically weighted regression (GWR) to model regional heterogeneity, using Statistics Korea microdata. `R` `GWR` `Spatial Statistics`

<details>
<summary><b>🏭 Industry–Academia Statistical Consulting</b></summary>

*   **Phototoxicity & eye-irritation alternative test methods**: Korea Testing & Research Institute (KTR) (2024). Inter-lab reproducibility across 4 labs (ICC, kappa; WLR/BLR 12/12), ROC-optimal cut-off (AUC 0.972), outlier-robust acceptance criteria (3-sigma, boxplot, medcouple)
*   **Eye-irritation international validation & skin-sensitization pre-validation**: KTR (Jul. 2026 – present). Statistical analysis for test method validation
*   **Oral mucosal irritation alternative test method (EpiOral™)**: Yonsei Univ. College of Dentistry (2025). Linear mixed models + ROC (Youden) to validate the 50% cut-off against OECD TG 439; ICC 0.997–1.000
*   **Fluid-bed coating process QC**: Kolon Pharmaceuticals (2025). 25 batches / 56K time-series records; Wilcoxon + BH correction, B-spline functional data analysis with bootstrap to find the process variables behind assay and dissolution drops
*   **Multiscale reconstruction and comparison of high-dimensional chromatin structure**: CNU (2024 – present). Hi-C contact-matrix preprocessing and multiscale structural analysis

</details>

* * *

### 🛠️ Tech Stack

**Languages**  
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![R](https://img.shields.io/badge/R-276DC3?style=flat-square&logo=r&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=mysql&logoColor=white)
![SAS](https://img.shields.io/badge/SAS-0766D1?style=flat-square)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![LaTeX](https://img.shields.io/badge/LaTeX-008080?style=flat-square&logo=latex&logoColor=white)

**ML / DL**  
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white)
![LightGBM](https://img.shields.io/badge/LightGBM-02569B?style=flat-square)
![YOLOv8](https://img.shields.io/badge/YOLOv8--Pose-111F68?style=flat-square&logo=ultralytics&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=flat-square&logo=opencv&logoColor=white)

**Tools & Serving**  
![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black)
![Flask](https://img.shields.io/badge/Flask-000000?style=flat-square&logo=flask&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)

* * *

### 🏆 Awards & Honors

*   🥇 **우수발표논문상**, 한국품질경영학회 (2026.05, 67편 중)
*   🥈 **논문발표상 장려상**, 한국데이터정보과학회 (2026.05, 46편 중)
*   💡 **창의상**, K-DATA SCIENCE 해커톤: **2024, 2025, 2026** (3년 연속)
*   🏅 **우수상**, 충남대 Data Science Challenge (2025.11)
*   🏅 **장려상 (구두논문·포스터논문 부문)**, 한국자료분석학회 (2025.11)
*   🏅 **학회장상**, 한국통계학회 (2025.02)
*   🎓 **석사 우수장학금 (이공계)**, 과학기술정보통신부 (2026.03 – 현재)

* * *

### 📜 Certifications

**Big Data Analysis Engineer (빅데이터분석기사)** · **SQLD** · **ADsP** · **Social Survey Analyst Lv.2 (사회조사분석사 2급)** · TOEIC 820 · TOEIC Speaking IH

* * *

### 🎓 Education

*   **M.S., Statistics & Data Science**, Chungnam National University (Mar. 2025 – Feb. 2027, expected)
*   **B.S., Information & Statistics**, Chungnam National University (Mar. 2021 – Feb. 2025)

* * *

### 📫 Contact

Feel free to reach out at [jiwonlim0492@gmail.com](mailto:jiwonlim0492@gmail.com). I write up paper reviews and debugging notes on my [blog](https://wony-wony.tistory.com).

Thanks for visiting! 🌱
