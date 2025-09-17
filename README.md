# IBM-x-Hactiv8-Data-Classification-and-Summarization-Capstone-Project-on-Bodyfat-Prediction
Capstone Project for Minicourse 

project_overview = f"""
# Body Fat Analysis: Regression + Quartile Classification + Auto-Summarization

## Objective
Memprediksi persentase body fat dan mengelompokkan individu ke dalam empat tingkat risiko (Low/Medium/High/VeryHigh) 
berdasarkan kuartil BodyFat%, lalu merangkum temuan secara otomatis menggunakan model summarization.

## Raw Dataset
Sumber: Kaggle (Body Fat). Sertakan tautan dataset asli pada README GitHub.

## Methods
- Regression: Linear Regression, RandomForestRegressor
- Classification: Logistic Regression, RandomForestClassifier (label dari kuartil BodyFat%)
- Preprocessing: imputasi median, standard scaling, train/test split stratified (untuk klasifikasi)
- Interpretability: korelasi & SHAP (opsional)
- Summarization: DistilBART (HuggingFace)

## Key Findings (ringkas)
{summary}

## Recommendations
{recs}
"""
