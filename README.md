# Prediksi Persentase Lemak Tubuh (Body Fat Prediction) dengan LLM IBM Granite 
Capstone Project for IBM x Hactiv8 Data Classification and Summarization Minicourse 


## Project Overview

Proyek ini bertujuan untuk menganalisis faktor-faktor antropometri yang paling berpengaruh terhadap persentase lemak tubuh (body fat). Dengan menggunakan dataset bodyfat dari Kaggle, analisis dilakukan untuk menemukan hubungan antara variabel seperti density, usia, berat badan, dan ukuran lingkar tubuh dengan persentase lemak tubuh. Pendekatan ini dapat memberikan wawasan penting dalam bidang kesehatan, kebugaran, dan penelitian medis terkait komposisi tubuh.

Selain itu, proyek ini memanfaatkan AI Agent (LangChain + LLM Replicate) untuk mempercepat eksplorasi data, pembuatan visualisasi, dan penyusunan insight.

## Raw Dataset Link

Dataset yang digunakan berasal dari Kaggle:
[BodyFat Prediction Dataset – Kaggle](https://www.kaggle.com/code/casper6290/bodyfat-prediction/input)

## Insight & Findings

Hasil analisis korelasi dan visualisasi menunjukkan:

1. Density memiliki korelasi negatif sangat kuat (\~−0.99) dengan BodyFat → semakin tinggi densitas tubuh, semakin rendah persentase lemak.
2. Abdomen (lingkar perut) adalah prediktor positif terkuat (\~0.8). Peningkatan lingkar perut secara signifikan meningkatkan persentase lemak tubuh.
3. Weight, Hip, dan Chest juga berhubungan positif dengan BodyFat (korelasi 0.6–0.7).
4. Age hanya memiliki hubungan lemah dengan BodyFat, menunjukkan faktor usia bukan determinan utama.
5. Model baseline menunjukkan bahwa Random Forest mengungguli model linear baik dalam regresi (lebih rendah RMSE) maupun klasifikasi (akurasi dan F1\_weighted lebih tinggi).

## AI Support Explanation

Dalam proyek ini, AI digunakan sebagai asisten analisis melalui:

* Proses analisis ini didukung oleh Large Language Model (LLM) ibm-granite/granite-3.3-8b-instruct yang digunakan melalui LangChain dan Replicate API.
* Mempercepat proses eksplorasi dengan code generation yang langsung dapat dijalankan di Colab.
* Menyediakan ringkasan insight dan rekomendasi dari hasil analisis numerik dan visualisasi.
