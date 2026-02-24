Parfait Omr 😄 ! On va faire **un portfolio GitHub clé en main**, prêt à copier-coller. Je te prépare **tous les README, mini datasets et pipelines Mermaid** pour tes 4 projets.

Tu n’auras qu’à créer ton repo `portfolio` et copier chaque dossier avec son contenu.

---

# **1️⃣ README général du repo `portfolio`**

`portfolio/README.md` :

```markdown
# Portfolio – Rosette-Michèle Otounga

Bienvenue sur mon portfolio GitHub ! 👩🏽‍💻

Je suis étudiante en Master Intelligence Artificielle et Data Scientist, avec expérience en **Big Data Engineering** et **Applied AI / ML**.

Ce repository présente mes 4 projets phares :

1. **Vision + LLM (Évaluation hallucinations)** – IA appliquée / ML / Computer Vision
2. **Benchmarking Cosmos World Models** – IA avancée / ML / Benchmarking
3. **Livraison de données à RTE** – Data Engineering / Data Delivery
4. **Automatisation panels Excel chez Renault** – Data Engineering / Industrialisation

Chaque projet inclut :
- README clair et complet
- Schéma de pipeline Mermaid
- Mini dataset simulé
- Méthodologie et résultats
```

---

# **2️⃣ Projet : Vision + LLM (Évaluation hallucinations)**

`portfolio/Vision_LLM/README.md` :

````markdown
# Vision + LLM (Évaluation hallucinations)

## 📌 Contexte
Projet IA appliquée pour évaluer les hallucinations d’un modèle multimodal Vision + LLM.
Objectif : fiabiliser les réponses générées et analyser les limites du modèle.

## 🧩 Problématique
Les LLM multimodaux peuvent produire des hallucinations ou erreurs factuelles.
Détecter et mesurer ces hallucinations est essentiel pour l’usage en production.

## ⚙️ Pipeline / Architecture
```mermaid
graph LR
A[Images d'entrée] --> B[Prétraitement]
B --> C[Modèle Recognize Anything + LLM]
C --> D[Sortie texte annoté]
D --> E[Analyse hallucinations]
````

## 🛠 Méthodologie

* Prétraitement des images (normalisation, redimensionnement)
* Génération de légendes / réponses avec LLM
* Évaluation des hallucinations avec métriques automatisées (precision, recall)
* Comparaison entre modèles et réglage hyperparamètres

## 📊 Dataset

* Mini dataset simulé : 5 images fictives + descriptions CSV
* Colonnes : image_id, description_attendue

## 🏆 Résultats / Livrables

* Tableau de métriques par image et modèle
* Graphiques : hallucinations les plus fréquentes
* Impact : meilleure compréhension des limites du modèle

## ⚠️ Limites / Perspectives

* Extension à d’autres types d’images
* Automatisation de la correction des hallucinations

## 💡 Recommandations / Next Steps

* Intégrer module de validation humaine
* Industrialiser pipeline sur serveur/cloud

````

`portfolio/Vision_LLM/mini_dataset.csv` :

```csv
image_id,description_attendue
img1.jpg,"Un chat sur un canapé"
img2.jpg,"Une voiture rouge sur la route"
img3.jpg,"Un chien qui joue avec une balle"
img4.jpg,"Un vélo devant une maison"
img5.jpg,"Une personne lisant un livre"
````

---

# **3️⃣ Projet : Benchmarking Cosmos World Models**

`portfolio/Benchmarking_Cosmos/README.md` :

````markdown
# Benchmarking Cosmos World Models

## 📌 Contexte
Projet avancé de ML pour comparer des modèles de World Modeling.
Objectif : créer un pipeline automatisé pour évaluer la performance et la robustesse des modèles.

## 🧩 Problématique
Les modèles de simulation doivent être comparables de manière **reproductible et scalable**.
Besoin de métriques standardisées et de tests automatisés.

## ⚙️ Pipeline / Architecture
```mermaid
graph LR
A[Modèles à tester] --> B[Préparation des jeux de données]
B --> C[Exécution automatique des modèles]
C --> D[Calcul des métriques comparatives]
D --> E[Tableau de benchmarking]
````

## 🛠 Méthodologie

* Standardisation des datasets
* Exécution de plusieurs modèles avec mêmes entrées
* Calcul automatique des métriques (MAE, RMSE, etc.)
* Génération de tableau comparatif et graphiques

## 📊 Dataset

* Mini dataset simulé : 5 lignes avec colonnes features et target
* Colonnes : state, action, reward, next_state

## 🏆 Résultats / Livrables

* Tableau de comparaison modèles
* Graphiques de performance
* Impact : industrialisation de l’évaluation et gain de temps

## ⚠️ Limites / Perspectives

* Ajouter plus de modèles
* Étendre aux datasets réels

## 💡 Recommandations / Next Steps

* Pipeline entièrement scalable sur serveur/cloud
* Intégration dans CI/CD pour tests réguliers

````

`portfolio/Benchmarking_Cosmos/mini_dataset.csv` :

```csv
state,action,reward,next_state
s1,a1,1,s2
s2,a2,0,s3
s3,a1,1,s4
s4,a2,0,s5
s5,a1,1,s1
````

---

# **4️⃣ Projet : Livraison de données à RTE**

`portfolio/Livraison_RTE/README.md` :

````markdown
# Livraison de données à RTE

## 📌 Contexte
Projet Data Engineering pour transformer et livrer des datasets fiables à RTE.
Objectif : traduire les besoins métier en pipeline SQL opérationnel.

## 🧩 Problématique
Les équipes métier ont besoin de données fiables et à jour.
Besoin d’un pipeline automatisé pour éviter erreurs manuelles.

## ⚙️ Pipeline / Architecture
```mermaid
graph LR
A[Requête métier] --> B[Extraction SQL]
B --> C[Transformation / nettoyage]
C --> D[Validation des données]
D --> E[Livraison dataset final]
````

## 🛠 Méthodologie

* Analyse des besoins métier
* Création de scripts SQL pour extraction et transformation
* Vérification des données (contrôles qualité)
* Livraison des datasets prêts à l’usage

## 📊 Dataset

* Mini dataset simulé : 5 lignes
* Colonnes : timestamp, voltage, current, power

## 🏆 Résultats / Livrables

* Dataset fiable livré aux équipes métier
* Process automatisé
* Impact : gain de temps et réduction des erreurs

## ⚠️ Limites / Perspectives

* Industrialiser pour d’autres départements
* Ajout de monitoring automatique

## 💡 Recommandations / Next Steps

* Intégration pipeline dans orchestration type Airflow

````

`portfolio/Livraison_RTE/mini_dataset.csv` :

```csv
timestamp,voltage,current,power
2025-01-01 00:00,230,5,1150
2025-01-01 01:00,231,4,924
2025-01-01 02:00,229,6,1374
2025-01-01 03:00,232,5,1160
2025-01-01 04:00,230,4,920
````

---

# **5️⃣ Projet : Automatisation panels Excel chez Renault**

`portfolio/Automatisation_Excel_Renault/README.md` :

````markdown
# Automatisation panels Excel chez Renault

## 📌 Contexte
Optimisation d’un workflow Excel pour Renault.
Objectif : réduire erreurs et temps passé à manipuler manuellement les panels.

## 🧩 Problématique
Workflow manuel sur Excel : répétitif, source d’erreurs.
Besoin d’un script ou macro pour industrialiser le process.

## ⚙️ Pipeline / Architecture
```mermaid
graph LR
A[Fichiers Excel bruts] --> B[Macro / Script VBA]
B --> C[Nettoyage & calculs automatiques]
C --> D[Panels consolidés prêts]
```
````

## 🛠 Méthodologie

* Analyse des panels existants
* Script VBA pour automatiser nettoyages, calculs et tableaux
* Test et validation des résultats sur mini dataset simulé

## 📊 Dataset

* Mini panel Excel : 5 lignes
* Colonnes : date, véhicule, consommation, distance, CO2

## 🏆 Résultats / Livrables

* Panels consolidés automatisés
* Réduction des erreurs et du temps de traitement
* Impact : workflow optimisé et industrialisé

## ⚠️ Limites / Perspectives

* Ajouter plus de règles métier

