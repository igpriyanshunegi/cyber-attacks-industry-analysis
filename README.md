# 🛡️ Cyber Attacks by Industry Sector — EDA Project

> A comprehensive Exploratory Data Analysis (EDA) of global cybersecurity threats from **2015 to 2024**, examining attack patterns, industry vulnerabilities, financial impact, and breach timelines.

**Author:** Priyanshu &nbsp;|&nbsp; **Domain:** IT Security / Cybersecurity Analytics &nbsp;|&nbsp; **Period Covered:** 2015–2024

[![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python)](https://www.python.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter)](https://jupyter.org/)
[![Pandas](https://img.shields.io/badge/Pandas-EDA-green?logo=pandas)](https://pandas.pydata.org/)
[![Plotly](https://img.shields.io/badge/Plotly-Interactive-purple?logo=plotly)](https://plotly.com/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

---

## 📑 Table of Contents

- [Project Overview](#-project-overview)
- [Problem Statement](#-problem-statement)
- [Dataset](#-dataset)
- [Project Objectives](#-project-objectives)
- [Key Findings & Insights](#-key-findings--insights)
- [Visualizations](#-visualizations)
- [Tech Stack](#-tech-stack)
- [Project Structure](#-project-structure)
- [How to Run](#-how-to-run)
- [Acknowledgements](#-acknowledgements)

---

## 🔍 Project Overview

The increasing frequency and sophistication of cyberattacks pose a critical challenge to organizations across all sectors. This project consolidates data-driven insights from a rich dataset spanning a decade of global cyber incidents to answer three fundamental questions:

- **Who** is being attacked (industries & countries)?
- **How** are they being attacked (attack types & vectors)?
- **What** does it cost — financially and operationally?

By conducting a structured EDA, this project helps cybersecurity teams, policymakers, and business leaders prioritize investments and build evidence-based defense strategies.

---

## ⚠️ Problem Statement

Despite extensive reports like the **Verizon DBIR** and open Kaggle datasets, there remains a gap in consolidated, actionable intelligence that reveals:

- Which industries face the **highest exposure** to cyberattacks
- What **attack types dominate** across different time periods
- How **breach timelines and resolution** vary by attack category
- What **economic and demographic** factors influence risk exposure

Without such analysis, organizations struggle to allocate security resources effectively, and cybersecurity teams lack the evidence base needed to defend against emerging threats.

---

## 📊 Dataset

| Property | Detail |
|---|---|
| **File** | `Global_Cybersecurity_Threats_2015-2024.csv` |
| **Records** | 3,000 incidents |
| **Time Period** | 2015 – 2024 |
| **Source** | Verizon DBIR / Kaggle |

### Columns

| Column | Type | Description |
|---|---|---|
| `Country` | Categorical | Country where the attack occurred |
| `Year` | Integer | Year of the incident (2015–2024) |
| `Attack Type` | Categorical | Type of attack (e.g., Phishing, Ransomware, DDoS) |
| `Target Industry` | Categorical | Industry sector targeted |
| `Financial Loss (in Million $)` | Float | Financial damage caused by the attack |
| `Number of Affected Users` | Integer | Number of users impacted |
| `Attack Source` | Categorical | Origin of the attack (e.g., Hacker Group, Nation State) |
| `Security Vulnerability Type` | Categorical | Exploited vulnerability (e.g., Unpatched Software, Weak Passwords) |
| `Defense Mechanism Used` | Categorical | Security measure in place (e.g., VPN, Firewall) |
| `Incident Resolution Time (in Hours)` | Integer | Time taken to resolve the incident |

---

## 🎯 Project Objectives

1. **Time-Series Analysis** — Uncover historical attack trends, seasonal patterns, and year-over-year shifts in threat intensity and financial damage.

2. **Industry Vulnerability Mapping** — Compare sectors (Finance, Healthcare, Retail, Government, IT, Education, Telecom) to identify those with the highest exposure and financial loss.

3. **Attack Type Profiling** — Analyze the relationship between attack categories, financial consequences, and incident resolution timelines.

4. **Correlation & Root Cause Analysis** — Apply heatmaps and statistical analysis to study the links between attack sources, vulnerabilities, defense mechanisms, and breach outcomes.

---

## 💡 Key Findings & Insights

### 🏭 Industry Targeting
- **IT sector** was the most targeted with **478 incidents**, followed by Banking (445) and Healthcare (429).
- Retail, Education, Government, and Telecom each recorded **400+ incidents**, highlighting that no sector is safe.
- The **Education sector** saw a notable spike in 2018 with 59 incidents in a single year.
- **Healthcare and Retail** show a gradual upward trend in attacks over the decade.

### 📈 Financial & Temporal Trends
- Financial losses show **significant volatility year-over-year**, reflecting the unpredictable nature of the threat landscape.
- Spikes in specific years correlate with the emergence of new ransomware strains and large-scale breaches.
- The total number of **affected users trended upward**, suggesting attackers are compromising increasingly larger datasets.

### ⚔️ Attack Type Analysis
- **Ransomware** is among the most financially devastating and operationally time-consuming attack types.
- Some attacks (e.g., Business Email Compromise) are **high-cost but quick to resolve** technically.
- **DDoS and spyware** attacks tend to be lower in direct financial cost but cause significant operational downtime.

### 🔗 Correlation Insights
- Financial loss and affected users show a **moderate-to-strong positive correlation** — larger breaches generally cost more.
- **Longer resolution times** are associated with higher financial losses, reinforcing the value of fast incident detection and response.

---

## 📊 Visualizations

| # | Chart | Type | Key Insight |
|---|---|---|---|
| 1 | Total Financial Loss Over Time | Line Chart | Year-over-year financial damage trend |
| 2 | Cyber Attacks by Sector & Year | Heatmap | Frequency matrix across industries |
| 3 | Total Attacks by Industry | Bar Chart | IT, Banking, Healthcare lead in frequency |
| 4 | Affected Users Over Time | Line Chart | Growth in breach scale |
| 5 | Average Users Affected by Industry | Horizontal Bar | Scale of impact per sector |
| 6 | Financial Loss vs Resolution Time | Grouped Bar | Cost-duration tradeoff by attack type |
| 7 | Correlation Heatmap | Heatmap | Relationships between key metrics |
| 8 | Total Financial Loss by Attack Type | Interactive Bar (Plotly) | Costliest attack categories |
| 9 | Cyber Attacks Over the Years | Interactive Line (Plotly) | Annual attack frequency trends |
| 10 | Attack → Industry → Country | Sunburst Chart (Plotly) | Hierarchical breakdown of global attacks |
| 11 | Financial Loss vs Affected Users | Scatter Plot (Plotly) | Attack impact distribution |

---

## 🛠️ Tech Stack

```
Python 3.x
├── pandas          — Data loading, cleaning, and aggregation
├── numpy           — Numerical computations
├── matplotlib      — Static charts and time-series plots
├── seaborn         — Heatmaps, bar plots, and statistical visualizations
└── plotly.express  — Interactive charts (sunburst, scatter, line)
```

---

## 📁 Project Structure

```
📦 cyber-attacks-industry-analysis/
 ┣ 📓 Cyber_Attacks_by_Industry_Sector.ipynb   ← Main analysis notebook
 ┣ 📄 Global_Cybersecurity_Threats_2015-2024.csv ← Dataset
 ┗ 📄 README.md                                 ← You are here
```

---

## 🚀 How to Run

### 1. Clone the repository

```bash
git clone https://github.com/igpriyanshunegi/cyber-attacks-industry-analysis.git
cd cyber-attacks-industry-analysis

```

### 2. Install dependencies

```bash
pip install pandas numpy matplotlib seaborn plotly jupyter
```

### 3. Launch the notebook

```bash
jupyter notebook Cyber_Attacks_by_Industry_Sector.ipynb
```

> Make sure `Global_Cybersecurity_Threats_2015-2024.csv` is in the **same directory** as the notebook before running all cells.

---

## 📌 Acknowledgements

- **Dataset Source:** [Kaggle](https://www.kaggle.com/) — Global Cybersecurity Threats 2015–2024
- **Domain Inspiration:** [Verizon Data Breach Investigations Report (DBIR)](https://www.verizon.com/business/resources/reports/dbir/)
- **Project by:** Priyanshu | [GitHub](https://github.com/igpriyanshunegi/cyber-attacks-industry-analysis)

---

<p align="center">
  <i>Built to turn raw threat data into actionable cybersecurity intelligence.</i><br/>
  ⭐ If you found this useful, consider starring the repo!
</p>
