# Project Panopticon: Intelligent Time-Series Proctoring AI

Project Panopticon is an ethical, high-precision time-series machine learning pipeline engineered to eliminate the "Blind Flagging" crisis in legacy remote proctoring systems. Developed during the iStudio AI Internship Capstone, this architecture systematically resolves false-positive triggers caused by environmental micro-noise (such as sneezing, blinking, or transient posture shifts) and addresses extreme class imbalances to safeguard honest students while upholding total exam integrity.

---

## 🛠️ The Core Engineering Challenges Solved

1. **The Asynchronous Data Trap:** Solved the complication of aligning data from fixed 1Hz video telemetry frequencies with highly irregular, action-triggered system event logs.
2. **Signal Jitter & Micro-Noise:** Built rolling statistics to filter out isolated environmental movements, preventing false accusations.
3. **Severe Class Imbalance:** Adjusted model penalties to handle datasets where roughly 98% of the records reflect entirely innocent student behavior.
4. **Ethical Decision Boundaries:** Moved the default classification boundary to a strict 90% certainty threshold to minimize false positives to near-zero.

---

## 📂 Repository File Structure

* `AI_student_code.ipynb` — The full, production-ready Jupyter Notebook detailing the data ingestion, feature engineering, and model validation pipeline.
* `video_telemetry.csv` — Time-series log capturing eye-gaze tracking and facial telemetry at a stable 1Hz frequency.
* `system_events.csv` — Log tracking asynchronous, event-driven activities such as tab switches and copy-paste inputs.
* `Project Panopticon_ Intelligent Proctoring AI.pptx` — The executive technical slide deck summarizing the capstone.

---

## ⚙️ Environment Setup & Dependencies

To replicate the project environment without needing a separate standalone file, install the necessary libraries using the embedded requirements listed below.

### Inline Requirements Spec (`requirements.txt`)
Ensure you are running Python 3.11+. You can copy and install these core libraries directly via pip:

```bash
pip install pandas numpy scikit-learn matplotlib seaborn jupyter
