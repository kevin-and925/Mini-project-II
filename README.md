# Mini-project-II
Système avancé d'analyse des sentiments utilisant RNN's

## Participants
OMOUALA André Kevin(OMOA15099900)
BOCOUM Aoua(BOCA65570200)
Agossou Fulbert(AGOF722040000)

## 1. Aperçu du projet et objectifs

Ce mini-projet a pour but de développer un système avancé d’analyse des sentiments 
appliqué à des critiques de films, en utilisant des techniques d’apprentissage profond,
plus précisément des réseaux de neurones récurrents (RNN) avec des couches Bidirectional LSTM.

L’objectif principal est de construire un modèle capable de classifier automatiquement une critique comme :

# positive 
# négative 

Ce projet couvre l’ensemble de la chaîne de traitement :

- préparation et prétraitement des données textuelles
- tokenisation et vectorisation des séquences
- conception et entraînement d’un modèle profond
- évaluation des performances
- mesure de l’empreinte carbone de l’entraînement
- explicabilité des prédictions avec **SHAP** et **LIME**
- réflexion sur les aspects éthiques
- aperçu du déploiement dans un contexte embarqué

---

## 2. Structure générale du projet

Les principales étapes réalisées dans ce projet sont les suivantes :

1. Préparation des données
2. Prétraitement du texte
3. Tokenisation et vectorisation des séquences
4. Conception et entraînement du modèle
5. Ajustement de certains hyperparamètres
6. Évaluation du modèle
7. Explicabilité avec SHAP et LIME
8. Considérations éthiques
9. Considérations de déploiement embarqué

# 3.  Instruction pour le téléchargement et le prétraitement des données

3.1 Pour ce projet, il faudrait tout d'abord commencer par vérifier si on a
instaler nos bibliothèques dans notre Anaconda prompt et aprés importer ces bliothèques qui sont :
`pip install numpy`
`pip install nltk`
`pip install shap`
`pip install matplotlib`
`pip install tensorflow`
`pip install scikit-learn`
`pip install lime`
`pip install codecarbon`

# 3.2 Téléchargement du dataset

téléchargement du fichier IMBD  sur le site indiquer: 
[[https://ai.stanford.edu/%7Eamaas/data/sentiment/](https://ai.stanford.edu/~amaas/data/sentiment/)]
il faut que l'utilisateur qui veut réaliser ce projet se rassure 
que ce fichier soit placer au bonne endroit. Par la suite il faut l'extraire 

## 3.3 Préparation des données et prétraitement du texte
Ici, voila ce qui est demander : 

- Charger et inspecter les données IMDB
- Convertir le texte en minuscule
- supprime les balises HTML
- supprime la ponctuation
- supprime les stopwords
- nettoyage du texte
- Convertir les avis en séquences numériques :
  # Positive = 1
  # Négative = 0


# 4 Tokenisation et vectorisation des séquences

Dans cette parties voici ce que l'on doit réalisées :
-On va faire la création d’un vocabulaire basé sur les mots les plus fréquents
-On va faire la génération d’un word index
-On fera la conversion des critiques en séquences d’entiers
-une application de padding pour rendre toutes les séquences de même longueur

## 5- Conception et entraînement du modèle
## 5.1- Architecture du modèle
Concernant la conception et l'entrainement on utilise le modéle RNN
qui est un réseau neuronal qui utilise : 

-une couche Embedding
-deux couches Bidirectional LSTM empilées
-Une couche Dense 
-Une couche Dropout
-une couche de sortie avec sigmaoid

## 5.2- Compilation du modéle
le Modéle a été compiler en utilisant optimizer(adam), le loss et metric(accuracy)

## 5.3- EarlyStopping
l'objectif de EarlyStopping est de limiter le surapprentissage autrement appeler **Overfitting** qui utilise les paramétres tel que (val_loss, patience...) pour arrêter l'entraînement

## 6- Étapes d’évaluation du modèle
Pour faire l'évaluation du modéle il va falloir utiliser certaines données de validation ainsi que les données de test.

## 7- Résultats de l’analyse de l’empreinte carbone
Dans ce projet, l’empreinte carbone de l’entraînement est mesurée à l’aide de la bibliothèque CodeCarbon.
Elle permet de faire des analyses afin de : 

-mieux comprendre le coût environnemental ;
-Comparer plusieurs approches selon leur efficacité énergétique;
-de sensibiliser aussi l’impact écologique des modèles d’IA

# 8- Considérations éthiques et méthodes d’explicabilité
# 8.1- Considérations éthiques
Dans ce projet on a plusieurs éthiques qui sont pris en compte tels que : 
-le dataset;
-Les erreurs de classification;
-La limitation du modéle
-l'importance d'avoir moins confiance a l'automatisation des avis;

# 8.2- Explicabilité
Pour mieux comprendre les décisions du modèle, des méthodes d’explicabilité sont utilisées, notamment :
-SHAP;
-LIME;
Ces outils permettent d’identifier quels mots ou quelles parties d’une critique influencent le plus la prédiction.

# 9- Aperçu du déploiement du système embarqué
Une partie du projet s’intéresse à la possibilité de déployer le modèle dans un environnement embarqué.
L'objectif est d'adapter le système afin qu’il puisse fonctionner 
sur une plateforme à ressources limitées, comme un microcontrôleur ou un dispositif embarqué.

Le déploiement sur un systéme embarqué impose plusieurs limites tels que:
-une mémoire restreinte;
-La capacité de calcul réduite;
-La consommation énergétique limitée;

# 10- Responsabilités liées à la publication du code
La publication de ce code source implique plusieurs responsabilités :

-On fourni un code clair, propre et compréhensible;
-On a documenter les étapes importantes du projet;
-On a éviter au maximun de publier des données sensibles ou non autorisées;
-On a signaler les limites du modèle;

# 11- Justification de la licence open-source

La licence choisie est la licence **MIT LICENSE**, parce que elle va permettre
a d'autres utilisateurs de s'en servir(Le code) et dans un cadre educatif de, le
modifier et l'ajouter dans d'autres projet. Cette licence est fortement favorable même sur le plan professionnelle.

# 12- Comparaison des pratiques de publication du code
La comparaison porte sur le Dépot public et le dépot, il faut savoir que le dépot public lui il favorise la transparence, la collaboration ainsi que la 
visibilité du projet. Tandis que le dépot privé limite l'accés et aussi 
réduit la transparence, la collaboration externe ainsi que la diffusion de 
certaines connaissances. 
Il faut aussi savoir que si un code un bien documenté il est plus facile a comprendre alors que si il est peu documentéil sera difficile a reproduire.










