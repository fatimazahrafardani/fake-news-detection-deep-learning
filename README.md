# 🧠 Fake News Detection باستخدام Machine Learning و Deep Learning

## 📖 Description
هذا المشروع يهدف إلى تصنيف الأخبار إلى **Fake (مزيفة)** أو **Real (حقيقية)** باستخدام تقنيات الذكاء الاصطناعي.

تم تطبيق نموذجين:
- نموذج تقليدي: TF-IDF + Logistic Regression
- نموذج متقدم: DistilBERT (Transformer)

المشروع يشمل جميع المراحل من معالجة البيانات إلى التقييم النهائي.

---

## 🎯 Objectives
- تحميل البيانات وتحليلها
- تنظيف البيانات (Preprocessing)
- القيام بـ Exploratory Data Analysis (EDA)
- بناء نموذج Machine Learning (TF-IDF)
- تدريب نموذج Deep Learning (DistilBERT)
- مقارنة الأداء بين النماذج

---

## 📊 Dataset
تم استخدام:
- Fake.csv
- True.csv

البيانات تحتوي على:
- title
- text
- subject
- date

تم دمج البيانات وإنشاء عمود جديد:
👉 content = title + text :contentReference[oaicite:0]{index=0}  

---

## ⚙️ Technologies Used
- Python
- Pandas / NumPy
- Scikit-learn
- Matplotlib
- Hugging Face Transformers
- PyTorch
- Google Colab (GPU)

---

## 🔄 Project Workflow

### 1. Data Loading
- تحميل البيانات من CSV
- التحقق من الأعمدة

### 2. Preprocessing
- إعطاء labels:
  - Fake = 1
  - Real = 0
- دمج البيانات وتنظيفها
- Train/Test Split مع stratification :contentReference[oaicite:1]{index=1}  

### 3. EDA
- توزيع البيانات (Fake vs Real)
- تحليل طول النصوص
- الكلمات الأكثر تكراراً :contentReference[oaicite:2]{index=2}  

### 4. Baseline Model
- TF-IDF Vectorization
- Logistic Regression

### 5. Deep Learning Model
- Tokenization باستخدام DistilBERT
- تدريب النموذج باستخدام Trainer API

### 6. Evaluation
- Accuracy
- Precision / Recall / F1-score
- Confusion Matrix

---

## 📈 Results

| Model | Accuracy |
|------|--------|
| TF-IDF + Logistic Regression | ~0.989 |
| DistilBERT | ~0.999 |

👉 DistilBERT أعطى أفضل النتائج :contentReference[oaicite:3]{index=3}  

---

## 📊 Model Comparison
- النموذج التقليدي جيد جداً
- لكن DistilBERT تفوق عليه بفضل فهم السياق (context)

---

## 🚀 How to Run

1. تثبيت المكتبات:
```bash
pip install pandas numpy scikit-learn matplotlib transformers torch
