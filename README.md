# 👁️ Project Panopticon: Intelligent Time-Series Proctoring AI

![Python](https://img.shields.io/badge/python-3.11+-blue.svg?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)
![Scikit-Learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white)
![Deployment Status](https://img.shields.io/badge/Deployment%20Status-GO-green?style=for-the-badge)

Project Panopticon is an ethical, high-precision time-series machine learning pipeline engineered to eliminate the **"Blind Flagging" crisis** in legacy remote proctoring systems. Developed during the iStudio AI Internship Capstone, this architecture systematically resolves false-positive triggers caused by environmental micro-noise (such as sneezing, blinking, or transient posture shifts) and addresses extreme class imbalances to safeguard honest students while upholding total exam integrity.

---

## 🛠️ The Core Engineering Challenges Solved

> 🚀 **The Objective:** Shift proctoring logic from volatile "instant triggers" to sustained "anomaly trends."

1. **The Asynchronous Data Trap:** Solved the complication of aligning data from fixed 1Hz video telemetry frequencies with highly irregular, action-triggered system event logs.
2. **Signal Jitter & Micro-Noise:** Built rolling statistics to filter out isolated environmental movements, preventing false accusations.
3. **Severe Class Imbalance:** Adjusted model penalties to handle datasets where roughly 98% of the records reflect entirely innocent student behavior.
4. **Ethical Decision Boundaries:** Moved the default classification boundary to a strict 90% certainty threshold to minimize false positives to near-zero.

---

## 📂 Repository File Structure

| File Name | Description | Type |
| :--- | :--- | :--- |
| 📄 `AI_student_code.ipynb` | Full production-ready interactive data science workflow. | Jupyter Notebook |
| 📊 `video_telemetry.csv` | Time-series log capturing eye-gaze tracking at 1Hz frequency. | Tabular Dataset |
| 📊 `system_events.csv` | Asynchronous log tracking event-driven actions (tab switches). | Tabular Dataset |
| 📉 `Project Panopticon_ Intelligent Proctoring AI.pptx` | Executive presentation deck demonstrating core outcomes. | PowerPoint |

---

## ⚙️ Environment Setup & Complete Tool Stack

To replicate the project environment without needing a separate standalone file, use the embedded configuration stack below. 

### Core Dependencies (`requirements.txt`)
```bash
pip install pandas numpy scikit-learn matplotlib seaborn jupyter
