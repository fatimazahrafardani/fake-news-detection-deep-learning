# 🧠 Détection des Fake News avec Machine Learning et Deep Learning

## 📖 Description
Ce projet vise à détecter automatiquement les fake news (fausses informations) en utilisant plusieurs approches de Machine Learning et Deep Learning.

Nous avons implémenté et comparé plusieurs modèles :
- TF-IDF + Régression Logistique
- CNN (Convolutional Neural Network)
- LSTM (Long Short-Term Memory)
- BERT (DistilBERT)

L’objectif est d’évaluer les performances de chaque modèle et identifier le plus performant.

---

## 🎯 Objectifs
- Nettoyer et préparer les données textuelles
- Réaliser une analyse exploratoire (EDA)
- Implémenter plusieurs modèles de classification
- Comparer les performances des modèles
- Optimiser la détection des fake news

---

## 📊 Dataset
Le dataset utilisé provient de Kaggle :
- Fake.csv → contient les fausses informations
- True.csv → contient les vraies informations :contentReference[oaicite:0]{index=0}  

Les données contiennent :
- title
- text
- subject
- date

Une nouvelle colonne a été créée :
👉 content = title + text

---

## ⚙️ Technologies utilisées
- Python
- Pandas / NumPy
- Scikit-learn
- TensorFlow / Keras
- PyTorch
- Hugging Face Transformers
- Matplotlib
- Google Colab (GPU)

---

## 🔄 Workflow du projet

### 1. Prétraitement des données
- Nettoyage du texte
- Suppression des doublons, URL, caractères spéciaux
- Conversion en minuscules
- Ajout des labels (Fake = 0, Real = 1)
- Fusion des datasets :contentReference[oaicite:1]{index=1}  

---

### 2. Analyse exploratoire (EDA)
- Distribution des classes (dataset équilibré)
- Analyse de la longueur des textes
- Analyse des sujets dominants (politicsNews) :contentReference[oaicite:2]{index=2}  

---

### 3. Modèles implémentés

#### 📌 1. TF-IDF + Régression Logistique
- Vectorisation du texte avec TF-IDF
- Modèle de classification classique

---

#### 📌 2. CNN
- Extraction des caractéristiques locales du texte
- Classification basée sur des motifs linguistiques :contentReference[oaicite:3]{index=3}  

---

#### 📌 3. LSTM
- Capture des dépendances séquentielles du texte
- Très adapté pour le traitement du langage naturel

👉 Accuracy ≈ 98.6% :contentReference[oaicite:4]{index=4}  

---

#### 📌 4. BERT (DistilBERT)
- Modèle Transformer pré-entraîné
- Fine-tuning sur le dataset
- Tokenization avec padding et truncation

👉 Meilleur modèle du projet :contentReference[oaicite:5]{index=5}  

---

## 📈 Résultats

| Modèle | Accuracy |
|--------|---------|
| Logistic Regression | ~0.98 |
| CNN | ~0.98 |
| LSTM | ~0.986 |
| BERT (DistilBERT) | ~0.999 |

👉 BERT offre les meilleures performances :contentReference[oaicite:6]{index=6}  

---

## 📊 Évaluation
- Matrice de confusion
- Accuracy
- Precision / Recall / F1-score

👉 Très peu d’erreurs pour tous les modèles  
👉 BERT est presque parfait

---

## 🔍 Comparaison des modèles
- Les modèles classiques sont performants
- Les modèles Deep Learning améliorent les résultats
- BERT dépasse tous les autres grâce à la compréhension du contexte

---

## 🚀 Comment exécuter le projet

1. Installer les dépendances :
```bash
pip install pandas numpy scikit-learn tensorflow torch transformers matplotlib
