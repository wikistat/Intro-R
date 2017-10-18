
##<a href="http://www.insa-toulouse.fr/" ><img src="http://www.math.univ-toulouse.fr/~besse/Wikistat/Images/Logo_INSAvilletoulouse-RVB.png" style="float:left; max-width: 80px; display: inline" alt="INSA"/> |  [*Mathématiques Appliquées*](http://www.math.insa-toulouse.fr/fr/index.html), [`Science des Données`](http://www.math.insa-toulouse.fr/fr/enseignement.html) 

# [R](https://cran.r-project.org/) pour Statistique et *Science des Données*

L'objectif de ces tutoriels, proposés sous forme de calepins ([*jupyter notebooks*](http://jupyter.org/)), est d'introduire les principaux concepts et fonctionnalités du langage [R](https://cran.r-project.org/) en insistant sur ceux indispensable au statisticien, maintenant *data scientist*. Syntaxe, objets et classes, fonctions graphiques, techniques de préparation (*munging* ou *wrangling*) des données puis leur analyse en enchaînant phases d'[exploration](http://wikistat.fr/) et de [modélisation](http://wikistat.fr/) ou [apprentissage](http://wikistat.fr/) (machine / statistique). Des exemples plus détaillés sur des données spécifiques (en R et en python) sont proposés sur [wikistat.fr](http://wikistat.fr/) ainsi que dans les autres dépôts de ce site. Les méthodes sont exposées dans les vignettes de [wikistat](http://wikistat.fr/).

Les documents sont des calepins (*notebooks*) au format .ipynb à télécharger et ouvrir dans *Jupyter*. Il suffit pour cela de cloner le dépôt dans son propre environnement [GitHub](https://github.com/) ou de télécharger l'archive zippée.

## Tutoriels d'initiation à [R](https://cran.r-project.org/)
- [`Cal1-start-R`](https://github.com/wikistat/Intro-R/blob/master/cal1-start-R.ipynb) Démarrrer avec R pour statisticien novice.
- [`Cal2-intro-R`](https://github.com/wikistat/Intro-R/blob/master/cal2-intro-R.ipynb) Introduction à R, ses objets, sa syntaxe.
- [`Cal3-graph-R`](https://github.com/wikistat/Intro-R/blob/master/cal3-graph-R.ipynb) Quelques graphiques avec R.
- [`Cal4-program-R`](https://github.com/wikistat/Intro-R/blob/master/cal4-program-R.ipynb) Eléments de programmation en R.



## Pourquoi [R](http://www.r-project.org/)?

Le logiciel R sous licence GNU  est facile à installer à partir de la page du [CRAN}(http://www.r-project.org/) ou d'un site miroir; ils contiennent toutes les ressources nécessaires à l'utilisateur de R, débutant ou expérimenté: fichiers d'installation, mises à jour, librairies, FAQ, newsletter, documentation... Il est le logiciel le plus utilisé de la communauté statistique académique et aussi de plus en plus dans les services R&D des entreprises industrielles en concurrence avec les logiciels commerciaux. Son utilisation nécessite un apprentissage à travers des tutoriels comme par exemple ceux de ce dépôt mais il est facile de démarrer à partir de quelques notions de base sur son utilisation;  de [*Start-R*](https://github.com/wikistat/Intro-R/blob/master/cal1-start-R.ipynb).

Dans sa structure, R est un langage de programmation *interprété*  d'une syntaxe voisine à celle du langage C et capable de manipuler des objets complexes sous forme de matrice, scalaire, vecteur, liste, facteur et aussi *data frame*. Proposant donc une *programmation matricielle*, il offre des fonctionnalités analogues à Matlab et dispose également d'une très riche librairie de quasiment toutes les procédures et méthodes statistiques de la littérature. Plus précisément, toutes les recherches récentes sont d'abord développées et diffusées à l'aide de ce logiciel par la communauté scientifique.

## Environnements d'Utilisation
Il existe de nombreuses librairies (cf. `Rcmdr`) d'interface graphique par menu mais celles-ci sont contraignantes, trop limitées dans les choix et options, elles ne peuvent éviter une utilisation par lignes de commandes; autant s'y mettre tout de suite, c'est le choix fait ici. 

Il existe également un environnement de programmation ou IDE*: [RStudio](http://www.rstudio.com/) relativement efficace; à l'utilisateur de faire ses choix. 

La présentation des tutoriels privilégie assez unanimement le format des calepins (notebook) Jupyter qui autorisent une exécution automatique et offrent la capacité d'intégrer chronologiquement des résutlats numériques, graphiques, des commentaires, au sein du même fichier.

C'est l'outil à privilégier pour promouvoir et diffuser les analyses statistiques d'une *recherche scientifique reproductible*.

## En résumé
- Installer la dernière version de [R](https://cran.r-project.org/)

Puis **au choix**

- Installer [RStudio](http://www.rstudio.com/)
- Copier, coller ou entrer successivement les commandes des tutoriels, 

**OU**

- [Installer Python](http://localhost:8888/notebooks/Intro-Python/Cal1-introPython.ipynb)
- Installer le noyau [IRkernel](https://irkernel.github.io/installation/). Dans le salles du CSN de l'INSA, exécuter les commandes suivantes après avoir ouvert R dans un terminal (pas Rstudio):
```bash
    R
```
```R
    install.packages(c('repr', 'IRdisplay', 'evaluate', 'crayon', 'pbdZMQ', 'devtools', 'uuid', 'digest'))
    library(devtools)
    withr::with_libpaths(new = "~/R/libs/", install_github('IRkernel/IRkernel'))
    IRkernel::installspec()
    quit() # quitter R
```
```bash
    jupyter notebook
```

**Dans les deux cas**

- Exécuter les cellules en analysant syntaxe et résultats
- Répondre aux questions, faire les exercices proposés

