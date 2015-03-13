Le logiciel libre Densidées calcule la densité des idées d'un texte (au sens de Kintsch 1974 et Turner & Greene 1977, c'est à dire le nombre moyen d'idées exprimées en 10 mots), utile en particulier pour l'analyse des discours de patients atteint de la maladie d'Alzheimer.

Un texte étiqueté par TreeTagger doit lui être fourni en entrée. La performance du logiciel a été évaluée dans l'article indiqué ci-dessous (Lee et al., RECITAL 2010) sur un corpus oral retranscrit de 13939 mots dont 5747 propositions. Les résultats de la version 1.2 présentent 2,7% de faux négatifs et 3,1% de faux positifs, soit un taux d'erreur de 0,5% sur le nombre de prédicats.

Densidées adapte à la langue française le calcul de densité d'idées implémenté pour la langue anglaise dans le logiciel [CPIDR](http://www.ai.uga.edu/caspr/), détaillé dans la publication suivante :
Cati Brown, Tony Snodgrass, Susan J. Kemper, Ruth Herman, et Michael A. Covington (2008) [Automatic measurement of propositional idea density from part-of-speech tagging](http://www.ai.uga.edu/caspr/BrownSnodgrassKemperHermanCovington2008.pdf). _Behavior Research Methods_ 40 (2) 540-545.

Il a été créé dans le cadre d'une collaboration issue de la [journée OSIDMESH](http://www.lirmm.fr/~semindoc/Osidmesh.html) d'octobre 2009, par [Hyeran Lee](http://www.univ-montp3.fr/praxiling/spip.php?article229) et [Philippe Gambette](http://igm.univ-mlv.fr/~gambette), doctorants des laboratoires [Praxiling](http://www.univ-montp3.fr/praxiling/) et [LIRMM](http://www.lirmm.fr) de Montpellier. [Melissa Barkat-Defradas](http://www.univ-montp3.fr/praxiling/spip.php?article22), Elsa Maillé et Constance Thuillier ont également contribué à la conception de ce logiciel, qui a donné lieu aux publications suivantes :
  * Hyeran Lee, Philippe Gambette, Constance Thuillier et Elsa Maillé (2010) [Densidées : calcul automatique de la densité des idées dans un corpus oral](http://halshs.archives-ouvertes.fr/halshs-00495768/fr/). _Actes de RECITAL 2010_.
  * Hyeran Lee, Philippe Gambette et Melissa Barkat-Defradas (2010) [Utilisation de l'analyse textuelle automatique dans la recherche sur la maladie d'Alzheimer](http://igm.univ-mlv.fr/~gambette/2010LeeGambetteBarkat.pdf). [Poster](http://igm.univ-mlv.fr/~gambette/2010LeeGambetteBarkatPoster.pdf) à _CEDIL 2010_.


[![](http://igm.univ-mlv.fr/~gambette/Densidees/LogoPraxiling.png)](http://recherche.univ-montp3.fr/praxiling)
[![](http://igm.univ-mlv.fr/~gambette/Densidees/LogoUm3.png)](http://www.univ-montp3.fr)
[![](http://igm.univ-mlv.fr/~gambette/Densidees/LogoLirmm.png)](http://www.lirmm.fr)
[![](http://igm.univ-mlv.fr/~gambette/Densidees/LogoUm2.png)](http://www.univ-montp2.fr)
[![](http://igm.univ-mlv.fr/~gambette/Densidees/LogoI2S.png)](http://www.edi2s.univ-montp2.fr)

## Installation et utilisation ##

Densidées est écrit en Python (version 2.6), il faut donc commencer par [télécharger Python](http://www.python.org/download/releases/2.6/) et l'installer (par exemple sous Windows) dans C:\Python26.

Puis, pour installer Densidées, téléchargez l'archive ZIP de la dernière version [sur la page des téléchargements](http://code.google.com/p/densidees/downloads/list), puis décompressez-la dans un répertoire quelconque de votre ordinateur.

Elle contient en particulier :
  * Densidees.exe, le programme à exécuter sous Windows
  * Densidees.py, le code du programme
  * ManuelDensidees.pdf, le manuel d'utilisateur, qui explique comment utiliser Densidées

Si vous voulez utiliser TreeTagger depuis le logiciel Densidées, il faudra également installer :
  * TreeTagger
  * Perl (par exemple sous Windows installer [Strawberry Perl](http://strawberryperl.com/), puis redémarrer l'ordinateur)


## Citation ##

Bien que Densidées soit un logiciel libre sous licence GPL, nous aimerions que vous fassiez référence à l'article suivant si vous l'utilisez dans une publication :
  * Hyeran Lee, Philippe Gambette, Constance Thuillier et Elsa Maillé. [Densidées : calcul automatique de la densité des idées dans un corpus oral](http://halshs.archives-ouvertes.fr/halshs-00495768/fr/). _RECITAL 2010_.


## Capture d'écran de l'interface Windows ##

[![](http://igm.univ-mlv.fr/~gambette/Densidees/Screenshot.png)](http://densidees.googlecode.com/files/ManuelDensidees.pdf)


## Versions ##

Version 1.3 (2010/06/30) :
  * appel automatique de TreeTagger depuis Densidées
  * mode "invisible" permettant de n'afficher que le résultat, en ligne de commande
  * calcul de la densité des idées comme ratio pour 10 mots selon la formule traditionnelle
  * amélioration des règles 208 et 701

Version 1.2 (2010/03/07) :
  * prétraitement des auxiliaires si pas fait par TreeTagger
  * 35 règles 001, 002, 020, 023, 024, 101, 102, 200, 054, 201, 202, 203, 204, 206, 207, 208, 210, 211, 212, 213, 214, 301, 302, 402, 405, 500, 509, 510, 512, 600, 601, 602, 701, 702, 703

Version 1.1 (2009/12/12) :
  * interface graphique
  * mode oral
  * affichage final du nombre de chacune des règles utilisées
  * 27 règles : 002, 020, 023, 024, 200, 054, 201, 202, 203, 204, 206, 207, 210, 211, 212, 213, 214, 301, 302, 402, 405, 500, 512, 600, 601, 602, 701

Version 1.0 (2009/11/21) :
  * texte étiqueté par TreeTagger en entrée du programme
  * 7 règles : 002, 003, 200, 201, 301, 302, 402
