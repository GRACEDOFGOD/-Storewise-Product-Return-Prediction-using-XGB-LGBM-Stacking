# 🛍️ ImpactStore Profit Prediction – Zindi Hackathon Submission

This project was developed as part of the **ImpactStore Hackathon**, hosted on [Zindi Africa](https://zindi.africa/). The goal was to build a predictive machine learning model that accurately estimates **Item-Store-Level Profit Returns** across a chain of Nigerian retail stores.

---

## 🙏 Dedication

> *This work is dedicated to **God Almighty**, the giver of wisdom, vision, and strength.*  
> *— Eniitan Oluwatoyin Shadrack*

---

## 📌 Problem Statement

Chief A. A. Babatunji, CEO of ImpactStore, wants to understand which combinations of products and stores yield the highest profit. This helps drive smart business decisions as the retail chain expands across Nigeria.

You are tasked with predicting the `Item_Store_Returns` using features like product type, weight, visibility, pricing, and store attributes (size, location, age, etc.).

---

## 💡 Solution Approach

The notebook features a **clean, high-signal machine learning pipeline** with:

- ✅ Smart missing value imputation  
- ✅ Sharp, minimalist feature engineering (no overfitting risk)  
- ✅ One strong encoding only: `Item_Type` → average return  
- ✅ Multiple base models trained with cross-validation  
- ✅ Stacking with RidgeCV for generalization  
- ✅ Clean `.csv` submission in Zindi format  

---

## 📂 Project Structure

| File                              | Description                                  |
|----------------------------------|----------------------------------------------|
| `Formatted_ImpactStore_Submission.ipynb` | 📓 Final Colab notebook (documented & clean) |
| `submission_r2_70_plus.csv`      | ✅ Prediction file (Zindi submission format)  |
| `README.md`                      | 📄 This documentation                        |

---

## 📈 Features Engineered

- `Store_Age`  
- `Price_per_kg`  
- `Visibility_Weight_Ratio`  
- `Price_Vis`  
- `Price_Weight`  
- `Item_Type_Encoded` *(target mean)*

> These were chosen for their **clarity, signal strength, and low risk of overfitting**.

---

## 🧠 Models Used

- `XGBoost`  
- `LightGBM`  
- `CatBoost`  
- `ExtraTrees`  
- `RidgeCV` (for model stacking)

---

## 🧪 Evaluation Metric

- R² Score (explained variance)  
- RMSE (prediction error)

---

## 🔧 How to Use

1. Clone the repo or download the notebook
2. Open in Google Colab or Jupyter
3. Upload the provided CSV files:
   - `train.csv`
   - `test.csv`
   - `SampleSubmission.csv`
4. Run all cells
5. Download the submission file

---

## 👨‍💻 Author

**Eniitan Oluwatoyin Shadrack**  
- 💬 Zindi: [@eniitans](https://zindi.africa/users/eniitans)  
- 📧 Email: *eniitanshad@gmail.com*  
- 🙏 Faith-first data scientist

---

## 📖 License

This project is open under the MIT License. Use it to learn, grow, and glorify God.

---

> _"Commit to the LORD whatever you do, and he will establish your plans." – Proverbs 16:3_
