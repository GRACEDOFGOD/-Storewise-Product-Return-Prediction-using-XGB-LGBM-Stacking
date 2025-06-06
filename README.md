# 🛍️ ImpactStore Profit Prediction Challenge – Final Submission

This repository contains the full machine learning pipeline developed for the **ImpactStore Hackathon**, a data science competition focused on predicting profit returns on products across multiple Nigerian retail stores.

The objective is to help ImpactStore identify which products, stores, and markets yield the highest returns. This enables better-informed decisions when expanding to new cities.

---

## 📌 Problem Statement

> Chief A. A. Babatunji, CEO of ImpactStore, seeks to understand profit behavior across his store network. Due to varying product prices and local market factors, the profit from the same product differs by store. Your task is to build a model that can accurately predict **Item_Store_Returns** based on product and store characteristics.

---

## 🧠 Solution Overview

The notebook includes:
- 🧹 **Data Cleaning & Preprocessing** – missing values imputed by groups
- 🧠 **Feature Engineering** – including group statistics, interaction terms, and log transforms
- 📈 **Modeling** – XGBoost, LightGBM, CatBoost, ExtraTrees with RidgeCV meta-stacking
- 🔗 **Stacking** – combines model predictions using RidgeCV for better generalization
- ✂️ **Postprocessing** – smart outlier handling and prediction capping
- 📊 **Evaluation** – performance metrics (R², RMSE) computed using OOF predictions
- 💾 **Submission** – predictions saved to `submission_r2_70_plus.csv`

---

## 📂 Files Included

| File                             | Description                                  |
|----------------------------------|----------------------------------------------|
| `Formatted_ImpactStore_Submission.ipynb` | 📓 Final Colab notebook (well documented)     |
| `submission_r2_70_plus.csv`     | ✅ Predicted returns (for Zindi submission)   |
| `README.md`                     | 📄 This documentation                         |

---

## 📊 Models Used

- `XGBRegressor`
- `LGBMRegressor`
- `CatBoostRegressor`
- `ExtraTreesRegressor`
- ➕ RidgeCV (for stacking meta-model)

---

## 🚀 How to Run

1. Clone or download this repo
2. Open `Formatted_ImpactStore_Submission.ipynb` in Google Colab
3. Upload your `train.csv`, `test.csv`, and `SampleSubmission.csv`
4. Run all cells
5. The notebook will auto-download the `submission_r2_70_plus.csv`

---

## 📈 Results

| Metric | Value (CV OOF) |
|--------|----------------|
| R²     | ~0.70+         |
| RMSE   | ~2500–2600     |

> Final submission optimized to reduce leaderboard error while maintaining generalization.

---

## 🏆 Author & Credits

- **Developer:** *[Your Name Here]*  
- **Platform:** [Zindi Africa](https://zindi.africa/)
- **Challenge:** [ImpactStore Hackathon](https://zindi.africa/competitions)

---

## 📬 Contact

- 💬 Zindi Username: `@YourZindiHandle`
- 📧 Email: your.email@example.com
- 🌐 GitHub: [github.com/yourusername](https://github.com/yourusername)

---

## 🔖 License

MIT License. You are free to use and adapt this code for educational or project purposes.
