# Mini-project-II
Système avancé d'analyse des sentiments utilisant RNN's

## Participants
OMOUALA André Kevin(OMOA15099900)
BOCOUM Aoua(BOCA65570200)
Agossou Fulbert(AGOF722040000)

## 1. Aperçu du projet et objectifs

Ce mini-projet a pour but de développer un système avancé d’analyse des sentiments appliqué à des critiques de films, en utilisant des techniques d’apprentissage profond, plus précisément des réseaux de neurones récurrents (**RNN**) avec des couches **Bidirectional LSTM**.

L’objectif principal est de construire un modèle capable de classifier automatiquement une critique comme :

- positive
- négative

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
3. **Tokenisation et vectorisation des séquences**
4. **Conception et entraînement du modèle**
5. **Ajustement de certains hyperparamètres**
6. **Évaluation du modèle**
7. **Explicabilité avec SHAP et LIME**
8. **Considérations éthiques**
9. **Considérations de déploiement embarqué**

# II-  Instruction pour le téléchargement et le prétraitement des données
Pour ce projet, il faudrait tout d'abord commencer par vérifier si on a
instaler nos bibliothèques dans notre Anaconda prompt et aprés importer ces bliothèques qui sont :
`pip install numpy`
`pip install nltk`
`pip install shap`
`pip install matplotlib`
`pip install tensorflow`
`pip install scikit-learn`
`pip install lime`
`pip install codecarbon`
Une fois les bibliothèques installer et vérifier, on va par la suite procéder
au téléchargement du fichier IMBD directement sur le site indiquer: 
[[https://ai.stanford.edu/%7Eamaas/data/sentiment/](https://ai.stanford.edu/~amaas/data/sentiment/)]
il faut que l'utilisateur qui veut réaliser ce projet se rassure 
que ce fichier soit placer au bonne endroit. Par la suite : 

## Préparation des données et prétraitement de texte : 

-le Nettoyage de texte(suppression des balises, conversion en minuscules, suppression de la ponctuation et des caractères spéciaux, ainsi que la suppression)


# III- Étapes de formation et d'évaluation 
Dans cet partie on va voir ce qui suit 

1-la division des données(il s'agit de séparer le dataset en ensemble d'entrainement)
2-formation des modéles(on parle des modéles classiques comme des modéles avancés)
3-l'évaluation(qui comprends les matrices de confusion, F1-Score, etc...)

## IV- Résultats de l'analyse de l'empreinte carbone
Dans notre Anaconda on déjà télécharger la bibliothèques adéquates. 
Son utilisation va nous permettre de mesurer l'impact énergetique
"from codecarbon import EmissionsTracker"

## V- Considérations éthiques et méthodes d'explicabilité
Ici il s'agit de respecter la vie privée des utilisateurs et de faire la prévention
des biais qui sont liés au genre, a la race ou à d'autres caractéristiques
pour mieux comprendre l'explicabilité on doit utiliser la bibliothèques
"import shap"

## VI- Aperçu du déploiement des sytèmes embarqués
On va faire la conversion du modèle qui sera comptabible avec un microcontrôleurs(Arduino)
en prenant en compte certaines contraintes du Arduino qui sont la limite de 
mémoire et tout ce qui l'entoure

## VII- Responsabilités liées à la publication du code :
7-1 Responsabiltés
-Garder un code propre, clair et qui fonctionne bien.
-Vérifie qu'il n'y a pas de données sensibles.
-être vigilant sur la reproductibilité des résultats.

7-2 Licences open source
-MIT License
-Cette license est utilisé parce que elle permet a d'autres : 
->De réutiliser le code
->De modifier le code

7-3 Pratique de publication
-A travers le dépôt public
-A travers la documentation

7-4 Protocole de signalement et correction des bogues
-Signaler un bug
-Créer une branche pour la correction Soumettre une pull request
-Mettre a jour la documentation 
-modifier la communauté des corrections majeures




