# 🚔 Navigating the Cyber Highway: Vehicle Cybersecurity Awareness Among Law Enforcement Officers

**Author:** Nandni Talreja  
**Institution:** UMass Amherst — Human Performance Lab  
**Supervisor:** Prof. Shannon Roberts  
**Period:** May 2023 – May 2024  
**Tools:** R (ggplot2, tidyverse) | Quarto | Logistic Regression | Survey Analysis | Driving Simulator

> **Associated Publication:** Jaji Pamarthi, William Hanson, Nandni Talreja, Meng Wang, Shannon C. Roberts. *"The effect of training on law enforcement response to vehicle cybersecurity events."* — presented to 30+ peers and decision-makers
> https://www.sciencedirect.com/science/article/pii/S2590198225003239#ak005

---

## 🔍 Project Overview

Modern police vehicles are increasingly connected — GPS, in-car computers, communication systems, and vehicle automation all create potential attack surfaces. Yet most law enforcement agencies have little to no structured training on vehicle cybersecurity. This study investigated whether targeted training could meaningfully change how Law Enforcement Officers (LEOs) perceive and respond to vehicular cyber threats.

Using a mixed-methods experimental design combining driving simulation, surveys, and interviews, this project measured the gap between officers who received specialized cybersecurity training versus a control group — and what that gap looks like in practice.

---

## ❓ The Problem

- Police vehicles are increasingly vulnerable to cyberattacks, yet **most agencies have no vehicle cybersecurity training**
- It was unknown whether targeted training could actually change LEO awareness and concern about cyber threats
- Demographic factors (age, experience, hours in vehicle) had never been systematically examined in relation to cybersecurity readiness in law enforcement

---

## 🧪 Study Design

14 Massachusetts Law Enforcement Officers participated (ages 27–51, avg. 17 years experience). Participants were randomly assigned to one of two groups:

| Group | Training Received |
|---|---|
| **Experimental** | Full cybersecurity training + 5 applied scenario exercises |
| **Sham (Control)** | General presentation without applied scenarios |

**Each participant completed 5 stages:**
1. Introduction to the vehicle and in-car systems
2. Cybersecurity training intervention (group-specific)
3. Three simulated drives — each containing a live cybersecurity event
4. Post-drive survey (demographics, cybersecurity knowledge, training feedback)
5. Structured interview about reactions and awareness

---

## 🛠️ What I Did

### Data Collection
- Recruited 14 LEOs through flyers, email outreach, and in-person visits to Massachusetts police stations
- Ran participants through a full-cab RTI driving simulator with embedded cyberattack events
- Collected multimodal data: reaction times, survey responses, and qualitative interview data

### Quantitative Analysis (R)
- **Descriptive statistics** and frequency distributions for all demographic variables (age, education, experience, hours in vehicle)
- **Grouped bar plots** comparing Experimental vs. Sham groups across key cybersecurity awareness variables
- **Correlation matrix** across 13 survey questions to identify relationships between demographics, experience, and cyber concern
- **Logistic regression (GLM, binomial family)** modeling the association between training group assignment and Q19: *"Are cyberattacks on police vehicles a serious concern for you?"*

### Qualitative Analysis
- Thematic coding of interview transcripts to surface patterns in officer reasoning, awareness gaps, and training preferences

---

## 📊 Key Findings

**Training increased concern about cyber threats.** The Experimental group reported higher concern about police vehicle cyberattacks than the Sham group — directionally supporting the hypothesis that applied training raises awareness.

**Cybercrime experience and training are linked.** Officers who had prior cybercrime training showed stronger awareness of cyber threats across multiple survey dimensions — an expected finding that was corroborated in interviews.

**Age showed a negative correlation** with perceived vehicle susceptibility (Q18) and cyberattack concern (Q19) — suggesting older, more experienced officers may be less attuned to emerging cyber risks, potentially due to familiarity with pre-connected vehicle systems.

**Gender showed unexpected negative correlations** across multiple survey items — a finding not anticipated by the research design and flagged as an area requiring further investigation with larger samples.

**Regression results were directionally significant but not statistically significant** (p = 0.121), which is expected given the small sample size (n=14). The GLM model confirms the study needs to be replicated at scale to draw firm causal conclusions.

**Bottom line:** The findings support building standardized vehicle cybersecurity training into law enforcement agencies — and suggest that applied, scenario-based components (not just informational presentations) are more likely to drive genuine awareness change.

---

## 📁 Repository Structure

```
├── analysis/
│   └── 604_Final_Project.qmd        # Full Quarto analysis: regression, correlations, visualizations
├── outputs/
│   ├── Talreja_604_Final_Poster.pdf  # Academic research poster (methods, results, conclusions)
│   └── Final_Presentation.pdf        # Slide deck presented to 30+ peers and faculty
└── README.md
```

---

## 📊 Sample Visuals

### Training Group Comparison — Cyberattack Concern (Q19)
*Experimental group officers showed notably higher concern about police vehicle cyberattacks after receiving scenario-based training, compared to the Sham (control) group.*

*(See poster PDF for full visualization)*

### Correlation Matrix — Key Highlights
- Cybercrime training and cybercrime experience are positively correlated with each other and with overall cyber concern
- Age is negatively correlated with Q18 (vehicle susceptibility) and Q19 (attack concern)
- Gender shows unexpected negative correlations across multiple awareness items

*(See `604_Final_Project.qmd` for full correlation matrix output)*

---

## ⚙️ How to Run

1. Clone this repository
2. Open `analysis/604_Final_Project.qmd` in RStudio
3. Install required packages:
```r
install.packages(c("tidyverse", "ggplot2", "kableExtra", "psych"))
```
4. Render the Quarto document to HTML or PDF

> ⚠️ **Note:** Raw participant data is not included due to IRB compliance and participant privacy agreements. The analysis code and outputs are provided for portfolio and reproducibility purposes.

---

## 🔒 Ethics & Compliance

This study was conducted under IRB-compliant protocols at UMass Amherst. All participants provided informed consent. No personally identifiable information is included in this repository. Participant recruitment involved in-person outreach to Massachusetts law enforcement agencies.

---

## 📚 Related Publication

This project contributed to a peer-reviewed publication on the broader law enforcement cybersecurity research program at the UMass Human Performance Lab:

> Jaji Pamarthi, William Hanson, **Nandni Talreja**, Meng Wang, Shannon C. Roberts. *"The effect of training on law enforcement response to vehicle cybersecurity events."*

---

## 📬 Contact

**Nandni Talreja**  
📧 talrejanandni.da@gmail.com  
🔗 [LinkedIn](https://linkedin.com/in/nandni-talreja)  
💼 [Upwork](https://www.upwork.com/freelancers/~01883ca0f5638a8066)
