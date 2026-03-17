# Fake News Detection using TF-IDF and DistilBERT

This project focuses on detecting fake news articles using two approaches:
1. A traditional Machine Learning baseline using TF-IDF + Logistic Regression
2. A Deep Learning approach using DistilBERT

## Dataset
The dataset contains two CSV files:
- Fake.csv
- True.csv

Each article includes:
- title
- text
- subject
- date

## Project Workflow
1. Data loading
2. Data preprocessing
3. Exploratory Data Analysis (EDA)
4. TF-IDF baseline model
5. DistilBERT fine-tuning
6. Final evaluation
7. Model comparison

## Results
- TF-IDF Accuracy: 98.92%
- DistilBERT Accuracy: 99.97%

## Key Findings
- The dataset is relatively balanced between fake and real news.
- DistilBERT outperformed the TF-IDF baseline.
- The confusion matrix showed very few classification errors.

## Files
- `Fake_News_Detection_Project.ipynb` : main notebook
- `Fake_News_Report_UPDATED.pdf` : final report
- `images/` : screenshots and visual outputs

## Tools and Libraries
- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Transformers
- Datasets
- PyTorch
## 🚀 Run on Google Colab

You can run this project directly on Google Colab:

👉 [Open in Colab](https://colab.research.google.com/drive/1yXV3_puvbFHP2_bYvrUvLVub28351-mY?usp=sharing)



## Author
FARDANI FATIMA ZAHRAE
