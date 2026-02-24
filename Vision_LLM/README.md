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
