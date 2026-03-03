## 📊 Étude de santé publique – Analyse des données alimentaires mondiales
### 📝 Contexte

Ce projet a été réalisé dans le cadre d’une étude de santé publique portant sur les données alimentaires mondiales de l’année 2017.
L’objectif est d’analyser les indicateurs liés à la sous-nutrition, à la disponibilité alimentaire et à l’aide alimentaire mondiale à partir de données fournies par la Organisation des Nations unies pour l'alimentation et l'agriculture (FAO).

### 🎯 Objectifs du projet

L’étude vise à répondre aux problématiques suivantes :

1. Calculer la proportion de personnes en état de sous-nutrition en 2017
2. Estimer le nombre théorique de personnes pouvant être nourries grâce à la disponibilité alimentaire mondiale
3. Effectuer le même calcul en se limitant aux produits d’origine végétale
4. Analyser l’utilisation de la disponibilité intérieure :
   - Alimentation humaine
   - Alimentation animale
   - Pertes

5. Identifier :
   - Les pays avec la plus forte proportion de sous-alimentation
   - Les pays ayant reçu le plus d’aide alimentaire
   - Les pays avec la plus forte/faible disponibilité alimentaire par habitant

### 🛠️ Technologies utilisées

Python 3

Jupyter Notebook

Pandas (manipulation de données)

NumPy

Matplotlib

Seaborn

### 📂 Jeux de données utilisés

Le projet repose sur 4 fichiers principaux :

Disponibilité alimentaire

17 variables

Données en kcal/personne/jour, protéines, milliers de tonnes, etc.

Population

Population exprimée en milliers d’habitants (convertie en habitants)

Aide alimentaire

Données converties en kilogrammes

Harmonisation des noms de colonnes

Sous-nutrition

Valeurs exprimées en millions d’habitants (converties en habitants)

Gestion des valeurs approximatives (<0.1 remplacé par 0)

🔎 Méthodologie
1️⃣ Nettoyage des données

Traitement des valeurs manquantes (fillna)

Conversion des unités (milliers → unités, millions → unités)

Harmonisation des noms de colonnes

Suppression des incohérences

2️⃣ Calcul de la sous-nutrition

Jointure des tables population et sous-nutrition pour calculer :

𝑃
𝑟
𝑜
𝑝
𝑜
𝑟
𝑡
𝑖
𝑜
𝑛
=
𝑁
𝑜
𝑚
𝑏
𝑟
𝑒
 
𝑑
𝑒
 
𝑝
𝑒
𝑟
𝑠
𝑜
𝑛
𝑛
𝑒
𝑠
 
𝑠
𝑜
𝑢
𝑠
 
𝑎
𝑙
𝑖
𝑚
𝑒
𝑛
𝑡
𝑒
ˊ
𝑒
𝑠
𝑃
𝑜
𝑝
𝑢
𝑙
𝑎
𝑡
𝑖
𝑜
𝑛
 
𝑡
𝑜
𝑡
𝑎
𝑙
𝑒
Proportion=
Population totale
Nombre de personnes sous aliment
e
ˊ
es
	​

3️⃣ Capacité théorique à nourrir la population mondiale

Conversion des disponibilités alimentaires en kcal totales :

𝐷
𝑖
𝑠
𝑝
𝑜
𝑛
𝑖
𝑏
𝑖
𝑙
𝑖
𝑡
𝑒
ˊ
 
𝑡
𝑜
𝑡
𝑎
𝑙
𝑒
=
𝑘
𝑐
𝑎
𝑙
/
𝑝
𝑒
𝑟
𝑠
/
𝑗
×
𝑝
𝑜
𝑝
𝑢
𝑙
𝑎
𝑡
𝑖
𝑜
𝑛
×
365
Disponibilit
e
ˊ
 totale=kcal/pers/j×population×365

Hypothèse retenue :
2500 kcal/jour/personne (moyenne des besoins journaliers)

Calcul du nombre théorique de personnes pouvant être nourries.

4️⃣ Analyse spécifique des céréales

Étude de la répartition entre :

🌾 Alimentation humaine

🐄 Alimentation animale

Céréales analysées :

Avoine

Blé et produits

Maïs et produits

Riz et produits

Orge et produits

Seigle et produits

Sorgho et produits

Millet et produits

Céréales, autres

Calcul des proportions :

Part destinée à l’alimentation humaine

Part destinée à l’alimentation animale

📈 Analyses complémentaires

Top 15 des pays avec la plus forte proportion de sous-alimentation

Top 15 des pays ayant reçu le plus d’aide alimentaire depuis 2013

Pays avec :

La plus forte disponibilité alimentaire par habitant

La plus faible disponibilité alimentaire par habitant

Étude de cas spécifique : Thaïlande et manioc

🚀 Résultats attendus

Ce projet permet de :

Mettre en évidence les déséquilibres alimentaires mondiaux

Évaluer la capacité théorique du système alimentaire mondial

Identifier les priorités géographiques en matière d’aide alimentaire

Comprendre la répartition entre alimentation humaine et animale
