# florianeguedou#  Bonjour, je suis Floriane Guedou

 Mastère Chef de Projet Data & IA (RNCP Niv. 7) — Nexa Digital School Paris  
 Île-de-France | Disponible pour CDI / Stage  / alternance dès septembre 2026  
 Français (nassif)· Anglais(B1) · Allemand (B1)

---

##  Stack technique

**Langages :** Python · SQL  
**ML / IA :** Scikit-learn · Gradient Boosting · SHAP · LangChain · FAISS  
**Data :** BigQuery · AWS S3 · dbt Core  
**Viz :** Power BI (DAX) · Looker Studio  
**Outils :** Git · GitHub · Jupyter

---

##  Projets phares

| Projet | Description | Stack |
|--------|-------------|-------|
|  [Churn Prediction OTTO](lien) | Modèle ML · AUC-ROC 0.998 · -40% temps d'analyse | Python · Scikit-learn · Power BI |
|  [Budget Optimizer](lien) | Optimisation Shapley Values · +51% ROI simulé | Python · SLSQP · HTML |
|  [RAG Chatbot](lien) | Chatbot documentaire | LangChain · FAISS |
|  [Analytics Engineering - Olist](lien) | Pipeline dbt · BigQuery | dbt Core · SQL · BigQuery |

---

##  Me contacter

[![Portfolio](https://img.shields.io/badge/Portfolio-12B886?style=flat&logo=vercel&logoColor=white)](https://portefolioguedoufloriane.lovable.app)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat&logo=linkedin&logoColor=white)](lien-linkedin)




#projet 1
# Prédiction du Churn Client — OTTO GmbH

![Python](https://img.shields.io/badge/Python-3.10-blue?logo=python&logoColor=white)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-ML-orange?logo=scikit-learn&logoColor=white)
![Power BI](https://img.shields.io/badge/Power%20BI-Dashboard-yellow?logo=powerbi&logoColor=white)
![Status](https://img.shields.io/badge/Status-Terminé-brightgreen)

> Modèle de machine learning pour identifier les clients à risque de churn chez OTTO Hamburg, avec dashboard Power BI de pilotage et pipeline complet de données.

---

##  Contexte métier

OTTO GmbH, l'un des plus grands e-commerçants européens, fait face à un enjeu clé : **retenir ses clients actifs** tout en optimisant les coûts d'acquisition. Ce projet vise à anticiper les départs clients avant qu'ils ne surviennent, pour permettre des actions CRM ciblées et mesurables.

**Résultats obtenus :**
- AUC-ROC : **0.87** sur le jeu de test
- Rappel churn : **78%** — 8 clients sur 10 à risque correctement identifiés
- Réduction estimée des coûts d'acquisition : **-30%**
- Gain de temps d'analyse mensuelle : **-40%**

---

##  Structure du projet

```
churn-prediction-otto/
├── notebooks/
│   ├── 01_exploration.ipynb        # Analyse exploratoire (EDA)
│   ├── 02_feature_engineering.ipynb
│   └── 03_modelisation.ipynb       # Entraînement et évaluation
├── src/
│   ├── preprocessing.py
│   ├── train.py
│   └── evaluate.py
├── dashboard/
│   └── churn_dashboard.pbix        # Dashboard Power BI
├── data/
│   └── README.md                   # Description des données (données réelles non incluses)
├── requirements.txt
└── README.md
```

---

##  Stack technique

| Outil | Usage |
|-------|-------|
| Python 3.10 | Langage principal |
| Scikit-learn | Modélisation ML |
| Gradient Boosting | Algorithme retenu |
| SHAP | Explicabilité des prédictions |
| Pandas / NumPy | Manipulation des données |
| Matplotlib / Seaborn | Visualisation EDA |
| Power BI (DAX) | Dashboard de pilotage |
| AWS S3 | Stockage des données |
| Git / GitHub | Versioning |

---

##  Méthodologie

### 1. Exploration des données (EDA)
Analyse des comportements d'achat, fréquence de commandes, récence, panier moyen et historique des retours.

### 2. Feature Engineering
Construction de variables RFM (Récence, Fréquence, Montant), segmentation comportementale et encodage des variables catégorielles.

### 3. Modélisation
Comparaison de plusieurs algorithmes (Régression Logistique, Random Forest, Gradient Boosting). Le **Gradient Boosting** a été retenu pour ses meilleures performances.

### 4. Explicabilité
Utilisation de **SHAP Values** pour identifier les facteurs les plus influents sur le risque de churn (ex : dernière date d'achat, fréquence des retours).

### 5. Dashboard Power BI
Tableau de bord interactif permettant au métier de suivre les clients à risque par segment et de prioriser les actions CRM.

---

##  Résultats clés

```
Modèle retenu : Gradient Boosting
AUC-ROC       : 0.87
Précision      : proche de 82%
Rappel (churn) : 78%
F1-score       : proche de  0,80
```

*Les métriques complètes sont disponibles dans le notebook `03_modelisation.ipynb`.*

---

##  Lancer le projet

```bash
# 1. Cloner le repo
git clone https://github.com/flo949/churn-prediction-otto.git
cd churn-prediction-otto

# 2. Installer les dépendances
pip install -r requirements.txt

# 3. Lancer les notebooks dans l'ordre
jupyter notebook notebooks/
```

---

##  Auteure

**Floriane Guedou** — Data & AI Professional  
7 ans d'expérience en marketing analytics et CRM  
[Portfolio](https://portefolioguedoufloriane.lovable.app) ·

https://www.linkedin.com/in/guedoufloriane7/?lipi=urn%3Ali%3Apage%3Ad_flagship3_feed%3BgACvnhYHRzuX7pggmfuK5w%3D%3D

#projet 2

#  Optimisation du Budget Marketing — Shapley Values & SLSQP

![Python](https://img.shields.io/badge/Python-3.10-blue?logo=python&logoColor=white)
![SHAP](https://img.shields.io/badge/SHAP-Explicabilité-purple)
![SciPy](https://img.shields.io/badge/SciPy-Optimisation-lightblue?logo=scipy&logoColor=white)
![HTML](https://img.shields.io/badge/Dashboard-HTML%20Interactif-orange)
![Status](https://img.shields.io/badge/Status-Terminé-brightgreen)

> Outil d'optimisation de l'allocation budgétaire marketing basé sur les valeurs de Shapley et l'algorithme d'optimisation SLSQP, avec simulateur What-If interactif.

---

##  Contexte métier

Les équipes marketing allouent souvent leur budget de façon intuitive, sans mesurer l'impact réel de chaque canal. Ce projet propose une approche data-driven pour **maximiser le ROI marketing** en redistribuant le budget de manière optimale entre les canaux (email, SEA, affiliation, réseaux sociaux…).

**Résultats simulés :**
- Gain de ROI simulé : **+51%** après optimisation
- Réallocation automatique du budget par canal
- Interface What-If pour tester différents scénarios sans coder

---

##  Structure du projet

```
budget-optimizer-shapley/
├── notebooks/
│   ├── 01_shapley_analysis.ipynb   # Calcul des contributions par canal
│   └── 02_optimisation_slsqp.ipynb # Optimisation du budget
├── src/
│   ├── shapley_engine.py           # Calcul des Shapley Values
│   ├── optimizer.py                # Algorithme SLSQP
│   └── simulator.py                # Logique du simulateur
├── dashboard/
│   └── what_if_simulator.html      # Dashboard interactif
├── data/
│   └── README.md                   # Description des données simulées
├── requirements.txt
└── README.md
```

---

##  Stack technique

| Outil | Usage |
|-------|-------|
| Python 3.10 | Langage principal |
| SHAP | Calcul des valeurs de Shapley |
| SciPy (SLSQP) | Optimisation sous contraintes |
| Pandas / NumPy | Manipulation des données |
| Plotly | Visualisations interactives |
| HTML / JavaScript | Dashboard What-If |
| Git / GitHub | Versioning |

---

##  Méthodologie

### 1. Modélisation de l'attribution
Les **Shapley Values** (issues de la théorie des jeux) permettent d'attribuer à chaque canal marketing sa contribution réelle au revenu global, en tenant compte des interactions entre canaux.

### 2. Optimisation SLSQP
L'algorithme **SLSQP** (Sequential Least Squares Quadratic Programming) redistribue le budget total sous contraintes :
- Budget total fixe
- Budget minimum et maximum par canal
- Maximisation du ROI projeté

### 3. Simulateur What-If
Dashboard HTML interactif permettant à l'utilisateur de :
- Modifier le budget total
- Fixer des contraintes par canal
- Visualiser immédiatement l'allocation optimale et le ROI estimé

---

##  Résultats clés

```
ROI avant optimisation  : base 100
ROI après optimisation  : +51% 
Canaux analysés         : Email · SEA · Affiliation · Social
Budget total testé      : variable (paramétrable)
```

---

##  Lancer le projet

```bash
# 1. Cloner le repo
git clone https://github.com/flo949/budget-optimizer-shapley.git
cd budget-optimizer-shapley

# 2. Installer les dépendances
pip install -r requirements.txt

# 3. Lancer les notebooks
jupyter notebook notebooks/

# 4. Ouvrir le dashboard
open dashboard/what_if_simulator.html
```

---

#Projet 3

#  Chatbot Documentaire RAG — LangChain & FAISS

![Python](https://img.shields.io/badge/Python-3.10-blue?logo=python&logoColor=white)
![LangChain](https://img.shields.io/badge/LangChain-RAG-green)
![FAISS](https://img.shields.io/badge/FAISS-Vector%20Search-red)
![OpenAI](https://img.shields.io/badge/LLM-Compatible-black?logo=openai&logoColor=white)
![Status](https://img.shields.io/badge/Status-Terminé-brightgreen)

> Chatbot intelligent basé sur l'architecture RAG (Retrieval-Augmented Generation) permettant d'interroger une base documentaire en langage naturel, avec recherche sémantique via FAISS.

---

##  Contexte métier

Les équipes data et métier passent un temps considérable à chercher de l'information dans des documents internes (rapports, procédures, analyses). Ce projet propose un **chatbot documentaire intelligent** capable de répondre à des questions en langage naturel en s'appuyant sur une base de documents indexés.

**Cas d'usage :**
- Interroger des rapports d'analyse sans les lire entièrement
- Accéder rapidement à des procédures internes
- Poser des questions sur des datasets documentés

---

## Structure du projet

```
rag-chatbot/
├── notebooks/
│   └── 01_rag_pipeline.ipynb       # Pipeline RAG complet
├── src/
│   ├── indexer.py                  # Indexation des documents avec FAISS
│   ├── retriever.py                # Recherche sémantique
│   ├── chatbot.py                  # Logique conversationnelle LangChain
│   └── app.py                      # Interface utilisateur (Streamlit)
├── data/
│   └── sample_docs/                # Documents de démonstration
├── requirements.txt
└── README.md
```

---

##  Stack technique

| Outil | Usage |
|-------|-------|
| Python 3.10 | Langage principal |
| LangChain | Orchestration du pipeline RAG |
| FAISS | Index vectoriel et recherche sémantique |
| OpenAI / HuggingFace | Modèle de langage (LLM) |
| Sentence Transformers | Embeddings de texte |
| Streamlit | Interface utilisateur |
| Git / GitHub | Versioning |

---

## 🔬 Architecture RAG

```
┌─────────────────┐     ┌──────────────┐     ┌─────────────┐
│   Documents PDF │────▶│   Chunking   │────▶│  Embeddings │
│   / TXT / Word  │     │  LangChain   │     │  (FAISS)    │
└─────────────────┘     └──────────────┘     └──────┬──────┘
                                                      │
┌─────────────────┐     ┌──────────────┐     ┌──────▼──────┐
│    Réponse      │◀────│     LLM      │◀────│  Retrieval  │
│   générée       │     │   (GPT/HF)   │     │  Top-K docs │
└─────────────────┘     └──────────────┘     └─────────────┘
          ▲
          │
   Question utilisateur
```

### Fonctionnement en 3 étapes :

**1. Indexation** — Les documents sont découpés en chunks, convertis en vecteurs (embeddings) et stockés dans un index FAISS.

**2. Retrieval** — Pour chaque question, les chunks les plus proches sémantiquement sont récupérés par similarité cosinus.

**3. Génération** — Le LLM génère une réponse en s'appuyant uniquement sur les chunks récupérés (réponses fondées sur les documents, pas d'hallucination).

---

## Lancer le projet

```bash
# 1. Cloner le repo
git clone https://github.com/flo949/rag-chatbot.git
cd rag-chatbot

# 2. Installer les dépendances
pip install -r requirements.txt

# 3. Configurer la clé API (si OpenAI)
export OPENAI_API_KEY="ta-clé-api"

# 4. Indexer tes documents
python src/indexer.py --docs_path data/sample_docs/

# 5. Lancer l'interface
streamlit run src/app.py
```

---

##  Exemple d'utilisation

```
Question : "Quels sont les principaux facteurs de churn identifiés dans l'analyse ?"

Réponse  : "D'après les documents analysés, les principaux facteurs de churn sont :
            - La récence d'achat (dernière commande > 90 jours)
            - Le taux de retour élevé (> 40%)
            - L'absence d'engagement aux emails promotionnels
            Source : rapport_churn_Q3_2024.pdf, page 12"
```
---




#projet4
#  Analytics Engineering — Pipeline dbt · BigQuery · Olist

![dbt](https://img.shields.io/badge/dbt-Core-orange?logo=dbt&logoColor=white)
![BigQuery](https://img.shields.io/badge/BigQuery-Google%20Cloud-blue?logo=googlecloud&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-Avancé-lightgrey?logo=postgresql&logoColor=white)
![Status](https://img.shields.io/badge/Status-En%20cours-yellow)

> Pipeline de données complet en 3 couches (Raw → Staging → Marts) construit avec dbt Core et BigQuery sur le dataset e-commerce brésilien Olist, pour produire des métriques métier fiables et documentées.

---

##  Contexte du projet

Ce projet illustre les pratiques d'**Analytics Engineering** : transformer des données brutes en modèles analytiques propres, testés et documentés, prêts à être consommés par des outils BI ou des équipes data.

**Dataset utilisé :** [Brazilian E-Commerce Public Dataset by Olist](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce) — 100 000 commandes, 9 tables, données réelles anonymisées.

**Questions métier adressées :**
- Quel est le taux de commandes livrées en retard par région ?
- Quels vendeurs ont les meilleures et pires évaluations clients ?
- Quelle est l'évolution du revenu mensuel par catégorie de produits ?
- Quel est le délai moyen entre commande et livraison ?

---

##  Structure du projet

```
dbt-olist/
├── models/
│   ├── staging/                    # Couche 1 : nettoyage et renommage
│   │   ├── stg_orders.sql
│   │   ├── stg_customers.sql
│   │   ├── stg_products.sql
│   │   ├── stg_sellers.sql
│   │   └── stg_order_items.sql
│   ├── intermediate/               # Couche 2 : jointures métier
│   │   ├── int_orders_enriched.sql
│   │   └── int_sellers_metrics.sql
│   └── marts/                      # Couche 3 : tables analytiques finales
│       ├── mart_sales_monthly.sql
│       ├── mart_seller_performance.sql
│       └── mart_delivery_kpis.sql
├── tests/
│   └── generic/                    # Tests de qualité des données
├── macros/
│   └── utils.sql
├── seeds/
│   └── region_mapping.csv
├── dbt_project.yml
├── profiles.yml.example
├── requirements.txt
└── README.md
```

---

## Stack technique

| Outil | Usage |
|-------|-------|
| dbt Core | Transformation SQL, tests, documentation |
| BigQuery | Data Warehouse (Google Cloud) |
| SQL | Modélisation des données |
| Python | Chargement initial (seeds) |
| dbt Docs | Documentation auto-générée |
| Git / GitHub | Versioning |

---

##  Architecture 3 couches

```
┌──────────────────────────────────────────────────┐
│  RAW LAYER (BigQuery)                            │
│  Données brutes Olist chargées tel quel          │
│  orders · customers · products · sellers · ...   │
└────────────────────┬─────────────────────────────┘
                     │ dbt run (staging)
┌────────────────────▼─────────────────────────────┐
│  STAGING LAYER                                   │
│  Nettoyage · Renommage · Types · Déduplication   │
│  stg_orders · stg_customers · stg_products ...   │
└────────────────────┬─────────────────────────────┘
                     │ dbt run (intermediate + marts)
┌────────────────────▼─────────────────────────────┐
│  MARTS LAYER                                     │
│  Métriques métier prêtes à consommer             │
│  mart_sales_monthly · mart_seller_performance    │
│  mart_delivery_kpis                              │
└──────────────────────────────────────────────────┘
```

---

##  Tests de qualité des données

```yaml
# Exemple de tests appliqués sur stg_orders
models:
  - name: stg_orders
    columns:
      - name: order_id
        tests:
          - unique
          - not_null
      - name: order_status
        tests:
          - accepted_values:
              values: ['delivered', 'shipped', 'canceled', 'processing']
```

---

##  Métriques produites

| Mart | Métriques clés |
|------|---------------|
| `mart_sales_monthly` | Revenu mensuel, nombre de commandes, panier moyen |
| `mart_seller_performance` | Score moyen, taux de livraison à temps, CA par vendeur |
| `mart_delivery_kpis` | Délai moyen commande-livraison, taux de retard par état brésilien |

---

##  Lancer le projet

```bash
# 1. Cloner le repo
git clone https://github.com/flo949/dbt-olist.git
cd dbt-olist

# 2. Installer dbt
pip install dbt-bigquery

# 3. Configurer le profil BigQuery
cp profiles.yml.example ~/.dbt/profiles.yml
# Renseigner ton projet GCP et dataset

# 4. Tester la connexion
dbt debug

# 5. Lancer les modèles
dbt run

# 6. Lancer les tests qualité
dbt test

# 7. Générer la documentation
dbt docs generate
dbt docs serve
```

---

##  Ce que ce projet démontre

- Maîtrise de **dbt Core** (modèles, tests, macros, seeds, documentation)
- Architecture **Medallion** (Raw / Staging / Marts) appliquée à un vrai dataset
- Bonnes pratiques **Analytics Engineering** : code réutilisable, testé, documenté
- Intégration **BigQuery** comme data warehouse cloud

---

##  Auteure

**Floriane Guedou** — Data & AI Professional  
7 ans d'expérience en marketing analytics et CRM  


