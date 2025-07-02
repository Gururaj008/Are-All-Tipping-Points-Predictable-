# 🌍 Are All Tipping Points Predictable?  
## A Test of Early Warning Signal Theory on Holocene Climate Events

![License](https://img.shields.io/badge/license-MIT-green) ![Python](https://img.shields.io/badge/python-3.8+-blue)  
**Author:** Gururaj H C  
**Status:** Research in Progress | Seeking Journal Publication

---

## 📌 Project Overview

Can abrupt climate shifts—known as **tipping points**—be predicted in advance?

This project puts **Early Warning Signal (EWS) Theory** to the test using real palaeoclimate data. By analyzing oxygen isotope records around major Holocene climate transitions, we assess the strength, reliability, and limitations of common statistical EWS indicators like autocorrelation and variance.

---

## 📂 Dataset

- **Source:** δ¹⁸O values from a palaeoclimate proxy record (e.g., ice cores or speleothems).
- **Format:** Tab-separated file `dataset.txt` with time (`age_calBP`) and proxy values (`d18O_vsmow`).
- **Events Studied:**
  - 🧊 Younger Dryas End (~11,700 BP)
  - 🌊 8.2k Event (~8,200 BP)
  - ☀️ Holocene Thermal Maximum Onset (~6,500 BP)

---

## ⚙️ What This Project Does

| Step | Description |
|------|-------------|
| 🧹 Preprocessing | Slice data ±2000 years around tipping events |
| 🧼 Detrending | Apply multiple methods (Gaussian, Savitzky-Golay, Spline, Differencing) |
| 📈 Metric Extraction | Compute AR1 and SD over sliding windows |
| 📊 Significance Testing | Use surrogate null models (N=300) |
| 🔥 Visualization | Generate heatmaps, plots, and statistical summaries |

---

## 🧠 Key Insights

- **Mixed Predictability:** Some events show clear EWS patterns (e.g., 8.2k), while others (e.g., HTM) do not.
- **Highly Method-Sensitive:** Choice of detrending method and window size significantly affects detection.
- **Not All Tipping Points Are Alike:** Uniform application of EWS theory may not work across different climatic transitions.

---

## 📁 Output

- **Figures**: All visuals saved in `/Final_Polished_Figures/`
- **Key Plots**: 
  - Kendall’s τ heatmaps for each event and method
  - Overlayed raw vs detrended signals
  - Surrogate vs actual signal comparisons

---


