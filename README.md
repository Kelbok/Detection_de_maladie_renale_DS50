# Prédiction de Maladie Rénale Chronique (CKD)

Application web interactive développée avec **Streamlit** pour explorer un jeu de données clinique, entraîner des modèles de classification et prédire la présence de **maladie rénale chronique (Chronic Kidney Disease – CKD)** à partir de nouveaux patients. :contentReference[oaicite:0]{index=0}  

---

## 🎯 Objectifs du projet

- Détecter précocement la maladie rénale chronique à partir de variables cliniques et biologiques.
- Construire un **pipeline complet** : nettoyage des données, exploration, modélisation, calibration des probabilités et prédiction sur de nouvelles données. :contentReference[oaicite:1]{index=1}  
- Proposer une interface simple pour des utilisateurs non techniques (médecins, analystes, étudiants).

---

## 🧠 Contexte métier

La maladie rénale chronique se caractérise par une dégradation progressive et irréversible de la fonction rénale, souvent asymptomatique aux premiers stades. Une détection précoce permet de ralentir la progression de la maladie et d’améliorer la qualité de vie des patients. :contentReference[oaicite:2]{index=2}  

L’application aide à classifier un patient en deux classes :

- `ckd` : patient atteint de maladie rénale chronique  
- `notckd` : patient non atteint

---

## 📊 Jeu de données

- **Nom** : Chronic Kidney Disease Dataset  
- **Source** : Kaggle – Mansoor Daku :contentReference[oaicite:3]{index=3}  
- **Taille** : 400 patients, 26 variables (25 explicatives + 1 cible)  
- **Type de tâche** : classification binaire (`ckd` / `notckd`)

Les variables incluent des mesures biologiques (créatinine, urée, sodium, potassium, hémoglobine, etc.) et des informations cliniques (hypertension, diabète, présence de bactéries, appétit, anémie…). :contentReference[oaicite:4]{index=4}  

---

## 🧮 Modèles de machine learning

Plusieurs classifieurs supervisés sont implémentés pour comparer les performances :

- Régression Logistique (*Logistic Regression*)
- Forêt Aléatoire (*Random Forest*)
- Machine à Vecteurs de Support – noyau RBF (*Support Vector Machine – SVM RBF*)
- K plus Proches Voisins (*K-Nearest Neighbors – KNN*)
- LightGBM


## Lancer l'application

```bash
pip install -r requirements.txt
streamlit run app/main.py
```
