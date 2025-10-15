# 🏉 United Rugby Championship Predictor (URC Predictor v1)

This notebook is a simple **United Rugby Championship match predictor** built in **Google Colab**.  
It automatically fetches fixtures, applies a basic predictive model, and outputs win probabilities and margins.

---

## ⚙️ Features

- Automatically fetches **upcoming URC fixtures** (from URC.com, FlashScore, or TheSportsDB)
- Includes a **basic predictive model** using:
  - Home advantage
  - Travel distance
  - Last year's team win rate
- Displays:
  - Fixture Date
  - Predicted Winner
  - Predicted Margin (points)
  - Win Probability (%)
  - Which data sources were used

---

## 🚀 How to Run

### Option 1 — Run in Google Colab

Click below to open and run directly in your browser:

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/trevorthackwell07/RugbyPredictor/blob/main/URC_Predictor_v1.ipynb)

Then in Colab:
1. Go to **Runtime → Run all**
2. Wait for the notebook to install dependencies and fetch fixtures
3. Scroll down to see predictions and download the results CSV if needed

---

## 🧠 Model Logic

The prediction is based on a simple scoring model:


Where:
- **Home Advantage** = +3.5 points  
- **Travel Penalty** = +2.0 points for South Africa ↔ Europe travel  
- **TeamStrengthDiff** = last year’s win rate difference  

---

## 🧾 Output Example

| Date       | Fixture             | Predicted Winner | Predicted Margin (pts) | Win Probability (%) | Sources Used     |
|-------------|--------------------|------------------|------------------------|---------------------|------------------|
| 2025-10-18  | Stormers vs Leinster | Leinster         | 2.4                    | 55.1                | FlashScore, URC  |
| 2025-10-19  | Bulls vs Munster     | Bulls            | 6.8                    | 72.3                | FlashScore, URC  |

---

## 📁 Repository Structure


---

## 🧩 Next Steps

- Add more data sources for accuracy (e.g., betting odds, form tables)
- Include model tuning or machine learning regression
- Automate weekly updates via GitHub Actions + email summary

---

## 🏆 Credits

Created by: **Trevor Thackwell**  
GitHub: [@trevorthackwell07](https://github.com/trevorthackwell07)  
Repository: [RugbyPredictor](https://github.com/trevorthackwell07/RugbyPredictor)  
Version: **v1 — Auto Fixtures + Basic Model (2025)**  
Last Updated: 2025-10-15
