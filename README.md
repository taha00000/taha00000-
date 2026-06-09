<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,50:1a1a2e,100:16213e&height=200&section=header&text=Taha%20Hunaid%20Ali&fontSize=48&fontColor=58a6ff&fontAlignY=38&desc=AI%20%2F%20ML%20Research%20Engineer%20%C2%B7%20Hardware%20Security%20%C2%B7%20Applied%20Cryptography&descSize=16&descAlignY=58&descColor=8b949e" />

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/taha-hunaid-072a55364/)
[![Portfolio](https://img.shields.io/badge/Portfolio-000000?style=for-the-badge&logo=vercel&logoColor=white)](https://taha00000.github.io/my-portfolio/)
[![Email](https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:tahahunaid@outlook.com)
[![CIRS Certified](https://img.shields.io/badge/CIRS-Certified-28a745?style=for-the-badge&logo=checkmarx&logoColor=white)](#)

</div>

---

## Who I Am

I am a **Computer Science student at Habib University** (Class of 2026, 3.71 GPA, 100% TOPS Scholar) working at the intersection of **interpretable machine learning**, **hardware-level cryptography**, and **applied cybersecurity**.

My work ranges from deploying production revenue-optimisation models at an automotive OEM, to designing NIST-standardised authenticated encryption in zero-unsafe embedded Rust, to threat-modelling HIPAA-compliant healthcare infrastructure from the ground up. I am a **Teaching Assistant for Cryptography and Network Security** and have led community digital-literacy programmes for 15 sessions.

> *I build things that are fast, provably secure, and explainable — from the silicon up.*

---

## Industry Experience

| Role | Organisation | Highlight |
|------|-------------|-----------|
| **Data Science Intern** | Indus Motors (Toyota Pakistan) | Deployed a revenue optimisation model yielding an estimated **PKR 1.49 B uplift** |
| **Teaching Assistant** | Habib University | Cryptography & Network Security — supported curriculum design and student mentorship |
| **Digital Literacy Lead** | Community Bootcamp | Ran a **15-session programme** for underserved learners |

---

## Featured Projects

### RustGuard — Memory-Safe ASCON-128 Authenticated Encryption for IoT

> **Rust · Embedded Systems · Cryptography · ARM Cortex-M4F · no_std**

Official implementation of the [NIST lightweight cryptography standard (NIST IR 8454)](https://csrc.nist.gov/pubs/ir/8454/final) in pure safe Rust, targeting ARM Cortex-M hardware with zero heap allocation. Paired with a custom **IoT Packet Authentication Protocol (RustGuard-PAP)** providing replay protection.

| Metric | Value |
|--------|-------|
| Unsafe code | **Zero** — `#![forbid(unsafe_code)]` compile-time enforced |
| Test suite | **24 / 24 tests pass** |
| ARM Cortex-M4F (32 B payload @ 16 MHz) | **2,303 cycles · 143.9 µs** |
| x86-64 encrypt (32 B) | **350 ± 192 ns** |
| Flash footprint (TM4C123) | **39,520 B** (15.4% of 256 KB) |
| Heap usage | **None** — `heapless` stack buffers only |

- Constant-time tag comparison via `subtle::ConstantTimeEq` — timing-attack resistant  
- Automatic key erasure via `zeroize::Zeroize` derived on internal state  
- Paper submitted to **NDSS 2027** (double-blind peer review)

[![RustGuard](https://img.shields.io/badge/RustGuard-View_Repo-orange?style=flat-square&logo=github)](https://github.com/taha00000/RustGuard)

---

### Interpretable Gearbox Fault Detection via Kolmogorov-Arnold Networks

> **Python · KAN · Signal Processing · Explainable AI · Predictive Maintenance**

First standalone application of **Kolmogorov-Arnold Networks (KAN)** to tabular gearbox fault data, benchmarked against seven classical ML classifiers. KANs replace fixed activation functions with learnable B-spline edges, enabling direct visualisation of feature relationships — no black box.

| Comparison | Result |
|------------|--------|
| Accuracy vs equivalent MLP (W=300) | **+5% improvement** |
| Baselines defeated | Decision Tree, Random Forest, SVM, Naive Bayes, KNN, Gradient Boosting, Logistic Regression |
| Interpretability | B-spline edge plots reveal threshold, sigmoid, or null feature roles |
| Pipeline stages | 5 reproducible scripts: validation → feature extraction → training → KAN optimisation → explainability |

- **Contributions:** first KAN paper on tabular vibration data; spline visualisation as a fault-diagnosis tool; KAN-driven network pruning validated across all baselines

[![KAN Fault Detection](https://img.shields.io/badge/KAN_Fault_Detection-View_Repo-blue?style=flat-square&logo=github)](https://github.com/taha00000/Interpretable-Gearbox-Fault-Detection-KAN)

---

### DVWA Penetration Testing Lab

> **Docker · OWASP Top 10 · Web Application Security · Exploit Analysis**

Containerised vulnerability assessment environment for systematic OWASP Top 10 exploit analysis. Full multi-level difficulty progression with documented attack chains, reproducible via Docker Compose.

- SQL Injection · XSS · CSRF · File Inclusion · Command Injection — all covered  
- Multi-level difficulty (Low → Medium → High → Impossible) with documented exploits  
- Designed for team-based security training and red-team practice

[![DVWA Lab](https://img.shields.io/badge/DVWA_Security_Lab-View_Repo-red?style=flat-square&logo=github)](https://github.com/taha00000/dvwa-security-lab)

---

### HIPAA Healthcare System — STRIDE Threat Model

> **Python · Security Architecture · STRIDE · IAM · Network Segmentation**

Secure-by-design architecture for a HIPAA-compliant healthcare appointment system. Full STRIDE threat modelling across patient/doctor portals, API gateway, and microservices handling PHI, PII, and financial data.

- **6 STRIDE threat categories** assessed with risk scores and mitigations  
- Controls: OAuth 2.0 + mandatory MFA · TLS 1.3 + AES-256 field-level encryption  
- Three-tier network segmentation · immutable audit trails · Infrastructure-as-Code deployment  
- Protects against spoofing, PHI disclosure, multi-tenant privilege escalation, and log repudiation

[![Threat Model](https://img.shields.io/badge/Hospital_Threat_Model-View_Repo-purple?style=flat-square&logo=github)](https://github.com/taha00000/hospital-secure-threat-model)

---

### Deep Reinforcement Learning — AI Models

> **Python · Jupyter · Reinforcement Learning · OpenAI Gym**

Exploration of deep reinforcement learning algorithms including policy gradient methods and Q-learning variants. Notebooks document training dynamics, reward curves, and agent behaviour analysis.

[![RL Models](https://img.shields.io/badge/RL_Models-View_Repo-yellow?style=flat-square&logo=github)](https://github.com/taha00000/AI-models-Reenforcment-learning-)

---

## Tech Stack

### Languages
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Rust](https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white)
![C++](https://img.shields.io/badge/C++-00599C?style=flat-square&logo=c%2B%2B&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![C#](https://img.shields.io/badge/C%23-239120?style=flat-square&logo=dotnet&logoColor=white)
![Verilog](https://img.shields.io/badge/Verilog-FF6600?style=flat-square&logo=xilinx&logoColor=white)
![LaTeX](https://img.shields.io/badge/LaTeX-008080?style=flat-square&logo=latex&logoColor=white)

### AI / ML / Data Science
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikit-learn&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=flat-square&logo=numpy&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=pandas&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=flat-square&logo=jupyter&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C?style=flat-square&logo=python&logoColor=white)

### Cybersecurity
![OWASP](https://img.shields.io/badge/OWASP_Top_10-000000?style=flat-square&logo=owasp&logoColor=white)
![STRIDE](https://img.shields.io/badge/STRIDE_Threat_Modelling-red?style=flat-square)
![ASCON](https://img.shields.io/badge/ASCON--128_(NIST_IR_8454)-lightgrey?style=flat-square)
![HIPAA](https://img.shields.io/badge/HIPAA_Compliance-0047AB?style=flat-square)
![Kali](https://img.shields.io/badge/Kali_Linux-557C94?style=flat-square&logo=kalilinux&logoColor=white)

### Infrastructure & Embedded
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazon-aws&logoColor=white)
![ARM Cortex](https://img.shields.io/badge/ARM_Cortex--M4F-0091BD?style=flat-square&logo=arm&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)

---

## GitHub Activity

<div align="center">

![GitHub Streak](https://streak-stats.demolab.com?user=taha00000&theme=github-dark-blue&hide_border=true&background=0d1117&stroke=1f6feb&ring=58a6ff&fire=ff6b35&currStreakLabel=58a6ff)

![Activity Graph](https://github-readme-activity-graph.vercel.app/graph?username=taha00000&theme=github-compact&bg_color=0d1117&color=58a6ff&line=1f6feb&point=58a6ff&area=true&hide_border=true)

![Commits](https://img.shields.io/badge/Total_Commits-177-58a6ff?style=flat-square&logo=github&logoColor=white)
![Repos](https://img.shields.io/badge/Public_Repos-17-1f6feb?style=flat-square&logo=github&logoColor=white)
![Stars](https://img.shields.io/badge/Stars_Earned-2-ffa500?style=flat-square&logo=github&logoColor=white)
![Since](https://img.shields.io/badge/On_GitHub_Since-2023-8b949e?style=flat-square&logo=github&logoColor=white)

</div>

---

## Credentials & Recognition

| Award / Certification | Detail |
|----------------------|--------|
| **CIRS Certified** | Industry-recognised information security certification |
| **Stanford International Program** | Accepted, 2023 |
| **100% TOPS Scholarship** | Habib University — merit-based full scholarship |
| **3.71 CGPA** | Top academic standing |
| **NDSS 2027 Submission** | Security research paper under double-blind review |

---

## What I Am Looking For

I am actively seeking **research-oriented internships and graduate opportunities** in:

- **AI / ML Engineering** — interpretable models, production ML, anomaly detection  
- **Systems Security** — embedded cryptography, secure protocol design, hardware security  
- **Applied Cybersecurity** — threat modelling, penetration testing, HIPAA/compliance engineering

> Open to full-time roles (post-graduation, 2026), research assistantships, and remote contracts.

---

<div align="center">

**tahahunaid@outlook.com** · [LinkedIn](https://www.linkedin.com/in/taha-hunaid-072a55364/) · [Portfolio](https://taha00000.github.io/my-portfolio/)

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:16213e,50:1a1a2e,100:0d1117&height=100&section=footer" />

</div>
