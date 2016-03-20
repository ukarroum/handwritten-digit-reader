# Lecteur de chiffre 

## Introduction 
Ce programme permet de lire des chiffres écrits à la main, c'est un tp que j'ai réalisé dans le cours de [Machine learning](https://www.coursera.org/learn/machine-learning) .

Le taux de reussite étant de *94.96%* .

Il utilise la regression logistique pour pouvoir entrainer 10 classificateurs (1 classificateur par chiffre) et choisit la réponse ayant la plus grande probabilité .

La fonction calculant le Cost et son Gradient est régularisé .

  
Pour plus d'informations : [Regression logistique](https://fr.wikipedia.org/wiki/R%C3%A9gression_logistique) .

Les classificateurs ont été entrainé par le [MNIST Database Of Handwritten digits](http://yann.lecun.com/exdb/mnist/)

## Fichiers du projet
Le TP contient en gros 8 fichiers :

* **displayData.m** : Permet d'afficher un echantillon du training Set .
* **ex3.m** : Le programme principale lance les entraineurs et calcule le taux de reussite de l'algorithme sur le dataset .
* **lrCostFunction** : Fonction calculant le cost ainsi que son gradient .
* **predictOneVsAll** : La fonction qui se charge de lire le digit, en gros elle renvoie le chiffre dont la probabilité est la plus grande .
* **sigmoid.m** : Calcule [La fonction Sigmoid](https://fr.wikipedia.org/wiki/Sigmo%C3%AFde_%28math%C3%A9matiques%29) .
* **ex3data1.mat** : Contient le dataset sous forme de deux matrices, l'une representant les images (en grayscale normalisé a [-1, 1] ) l'autre les labels representé par chaque image .
* **fmincg.m** : La fonction qui se charge de la minimisation du cost .
* **oneVsAll** : Se charge d'entrainer les 10 calssificateurs via regression logistique .


