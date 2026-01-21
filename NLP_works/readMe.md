## Étape 1 : Préparer l'environnement
*************************************************************************************
1. Installer Python :
Assurez-vous d'avoir Python 3.8 ou une version ultérieure installé sur votre machine.
Téléchargez-le depuis python.org si nécessaire.

2. Installer les bibliothèques nécessaires :
Le fichier requirements.txt contient toutes les dépendances. Installez-les avec : pip install -r requirements.txt

## Étape 2 : Préparer les données
*************************************************************************************
Téléchargez le dataset :

Téléchargez le jeu de données  Amazon Fine Food Reviews, récupérez-le depuis Kaggle. (nous n'avons utiliser que les 10 000 premières observations du dataset)
Placez le fichier des données : Placez le fichier CSV dans le même dossier que le script Python.
Assurez-vous que le nom du fichier correspond à celui attendu par le script (par exemple : Reviews.csv).

## Étape 3 : Lancer le script
************************************************************************************
Exécuter le script principal : dans le terminal ou un IDE (comme VSCode ou PyCharm), lancez le script 
Les résultats seront imprimés dans la console et enregistrés dans un fichier results.txt.

## Étape 4 : Analyser les résultats
************************************************************************************
Fichier results.txt : Consultez ce fichier pour voir les performances de chaque méthode de tokenization (précision, rappel, score F1, exactitude).

## Étape 5 : Résolution des problèmes (si nécessaire)
**********************************************************************************
* Problème de mémoire :
Si vous rencontrez des erreurs liées à la mémoire (MemoryError), réduisez la taille des données ou utilisez l'option max_features dans CountVectorizer :
vectorizer = CountVectorizer(max_features=5000)
* Erreur liée au dataset :
Vérifiez que les colonnes du dataset sont bien nommées (Text et Score).
* Installation des bibliothèques :
Si des bibliothèques manquent, installez-les individuellement :
pip install nom_de_la_bibliotheque
