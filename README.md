****** README DENSIDEES ******

Le logiciel libre Densid�es calcule la densit� des id�es d'un texte (au sens de Kintsch 1974 et Turner & Greene 1977, c'est � dire le nombre moyen d'id�es exprim�es en 10 mots), utile en particulier pour l'analyse des discours de patients atteint de la maladie d'Alzheimer.

Un texte �tiquet� par TreeTagger doit lui �tre fourni en entr�e. La performance du logiciel a �t� �valu�e dans l'article indiqu� ci-dessous (Lee et al., RECITAL 2010) sur un corpus oral retranscrit de 13939 mots dont 5747 propositions. Les r�sultats de la version 1.2 pr�sentent 2,7% de faux n�gatifs et 3,1% de faux positifs, soit un taux d'erreur de 0,5% sur le nombre de pr�dicats.

Densid�es adapte � la langue fran�aise le calcul de densit� d'id�es impl�ment� pour la langue anglaise dans le logiciel CPIDR (http://www.ai.uga.edu/caspr/), d�taill� dans la publication suivante :
Cati Brown, Tony Snodgrass, Susan J. Kemper, Ruth Herman, et Michael A. Covington (2008) [http://www.ai.uga.edu/caspr/BrownSnodgrassKemperHermanCovington2008.pdf Automatic measurement of propositional idea density from part-of-speech tagging]. Behavior Research Methods 40 (2) 540-545.

Il a �t� cr�� dans le cadre d'une collaboration issue de la journ�e OSIDMESH (http://www.lirmm.fr/~semindoc/Osidmesh.html) d'octobre 2009, par Hyeran Lee (http://www.univ-montp3.fr/praxiling/spip.php?article229) et Philippe Gambette (http://www.lirmm.fr/~gambette), doctorants des laboratoires Praxiling (http://www.univ-montp3.fr/praxiling/) et LIRMM (http://www.lirmm.fr) de Montpellier. Melissa Barkat-Defradas (http://www.univ-montp3.fr/praxiling/spip.php?article22), Elsa Maill� et Constance Thuillier ont �galement contribu� � la conception de ce logiciel, qui a donn� lieu aux publications suivantes :
 * Hyeran Lee, Philippe Gambette, Constance Thuillier et Elsa Maill� (2010) [http://halshs.archives-ouvertes.fr/halshs-00495768/fr/ Densid�es : calcul automatique de la densit� des id�es dans un corpus oral]. Actes de RECITAL 2010.
 * Hyeran Lee, Philippe Gambette et Melissa Barkat-Defradas (2010) [http://www.lirmm.fr/~gambette/2010LeeGambetteBarkat.pdf Utilisation de l'analyse textuelle automatique dans la recherche sur la maladie d'Alzheimer]. Poster � CEDIL 2010 (http://www.lirmm.fr/~gambette/2010LeeGambetteBarkatPoster.pdf).


== Installation et utilisation ==

Densid�es est �crit en Python (version 2.6), il faut donc commencer par [http://www.python.org/download/releases/2.6/ t�l�charger Python] et l'installer (par exemple sous Windows) dans C:\Python26.

Puis, pour installer Densid�es, t�l�chargez l'archive ZIP de la derni�re version [http://code.google.com/p/densidees/downloads/list sur la page des t�l�chargements], puis d�compressez-la dans un r�pertoire quelconque de votre ordinateur.

Elle contient en particulier :
 * Densidees.exe, le programme � ex�cuter sous Windows
 * Densidees.py, le code du programme
 * ManuelDensidees.pdf, le manuel d'utilisateur, qui explique comment utiliser Densid�es

Si vous voulez utiliser TreeTagger depuis le logiciel Densid�es, il faudra �galement installer :
 * TreeTagger
 * Perl (par exemple sous Windows installer Strawberry Perl http://strawberryperl.com, puis red�marrer l'ordinateur)


== Citation ==

Bien que Densid�es soit un logiciel libre sous licence GPL, nous aimerions que vous fassiez r�f�rence � l'article suivant si vous l'utilisez dans une publication :
 * Hyeran Lee, Philippe Gambette, Constance Thuillier et Elsa Maill�. [http://halshs.archives-ouvertes.fr/halshs-00495768/fr/ Densid�es : calcul automatique de la densit� des id�es dans un corpus oral]. RECITAL 2010.


== Versions ==

Version 1.3 (2010/06/30) :
 * appel automatique de TreeTagger depuis Densid�es
 * mode "invisible" permettant de n'afficher que le r�sultat, en ligne de commande
 * calcul de la densit� des id�es comme ratio pour 10 mots selon la formule traditionnelle
 * am�lioration des r�gles 208 et 701

Version 1.2 (2010/03/07) :
 * pr�traitement des auxiliaires si pas fait par TreeTagger
 * 35 r�gles 001, 002, 020, 023, 024, 101, 102, 200, 054, 201, 202, 203, 204, 206, 207, 208, 210, 211, 212, 213, 214, 301, 302, 402, 405, 500, 509, 510, 512, 600, 601, 602, 701, 702, 703

Version 1.1 (2009/12/12) :
 * interface graphique
 * mode oral
 * affichage final du nombre de chacune des r�gles utilis�es
 * 27 r�gles : 002, 020, 023, 024, 200, 054, 201, 202, 203, 204, 206, 207, 210, 211, 212, 213, 214, 301, 302, 402, 405, 500, 512, 600, 601, 602, 701
 
Version 1.0 (2009/11/21) :
 * texte �tiquet� par TreeTagger en entr�e du programme
 * 7 r�gles : 002, 003, 200, 201, 301, 302, 402

