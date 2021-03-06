# Chroniques Oubliées Contemporain

_A french Contemporary RPG based on the D20 system / OGL 3.5._

Chroniques Oubliées Contemporain est un jeu de r&ocirc;le doté d'un système simple mais complet bas&eacute; sur le syst&egrave;me d20/OGL 3.5.

Cette feuilles de personnage inclut quelques jets et r&egrave;gles optionnelles.

Le jeu complet est disponible sur le site de l'éditeur [Black Book Editions](http://www.black-book-editions.fr/produit.php?id=4349).

# Version courante
2.4 [Screenshot](coc_v2.png)

# Notes de version

## v2.4 (2019-01-01)
* Fiche de personnage avec sélection du type par dropdown (PJ, PNJ ou Véhicule)
* Modification cosmétique de la fiche avec une bordure aux coins arrondis
* Plus de case Traits/Langues/Niveau de vie sur l'onglet Caractéristiques. Ces informations peuvent être indiquées dans la liste répétable des traits de l'onglet Capacités
* Ajout d'un sheet-worker permettant de détecter si le personnage a subi une blessure grave, quand il perd en une seule fois un nombre de PV supérieur au seuil. La case Blessure est automatiquement cochée et l'état préjudiciable Affaibli activé.
* Ajout d'une case à cocher COCY à côté de l'initiative permettant de gérer les multiples actions par round en Cyberpunk. Après avoir lancé l'initiative, le fait de cocher cette case permet au rang d'initiative du personnage de diminuer de -10 à chaque fois qu'un jet d'attaque est réalisé via la fiche.
* Les Traits sur l'onglet Capacités sont maintenant affichés en permanence
* Possibilité de faire un jet de PC sur l'onglet Equipement qui ne fait qu'un affichage dans le chat
* Trois choix d'initiative dans l'onglet Configuration : normale (init), variable (init + 1d6 explosif), cyberpunk (init + 1d6 explosif, résultat final limité à init de base x 2)
* Ajout de champs dans l'onglet Configuration permettant d'indiquer le bonus de PC ainsi que de les nommer (Points de Choc en Horreur, Points de Cash en Cyberpunk, Points de Chance chargé par défaut à la première ouverture de la fiche)
* Ajout de cases à cocher sur les lignes d'armes/attaques permettant de faire un jet d'attaque sans jet de dommages ou un jet de dommages sans jet d'attaque (fiches PJ et PNJ)
* Ajout d'une option Choix dans les Mods et Mods de test des jets de capacités permettant de choisir la caractéristique à utiliser au moment du jet
* Import du Statblock pour les PNJs
* Ajout d'une fiche de véhicule avec caractéristiques de base et liste répétable de jets permettant d'inclure les caractéristiques de véhicule et celles du personnage (pas de solution satisfaisante trouvée pour aller chercher les caractéristiques de la fiche du pilote dont le nom est indiqué)
* Modification cosmétique avec une bordure aux coins arrondis et un affichage élargi dans les rolls template
* Nouveau tag {{portee= }} permettant d'afficher la portée d'une arme à distance
* Modification du roll-template pour permettre l'affichage d'un jet de dommages même sans jet d'attaque préalable


## V2.3 (2018-12-13)
* Correction d'un bug sur le calcul des buffs Divers ATD et DEF

## v2.2 (2018-12-11)
* Modification du bouton de jet d'attaque pour générer un attribut pour chaque ligne. 
* Correction des espaces dans la commande invoquée par le bouton d'attaque pour en permettre l'utilisation à la fois dans le chat et via l'API en appelant la pseudo ability %{nom|repeating_armes_$n_jet} (où n est le no de ligne, base 0)
* Nommage du checkbox "Plus de voies" (@{voies789}) afin de préserver son état d'un appel à un autre de la fiche de personnage. Ce changement a été oublié dans les commits de la Version 2.1
* Modification du bouton de jet de capacité pour générer un attribut pour chaque ligne. 
* Correction des espaces dans la commande invoquée par le bouton de jet de capacité pour en permettre l'utilisation à la fois dans le chat et via l'API en appelant la pseudo ability %{<nom du personnage>|repeating_jetcapas_$n_jet} (où n est le no de ligne, base 0) 
* Modification mineures des textes dans le sélecteur du type de jet de capacité
* Ajout d'un groupe d'options "Attaques" dans le sélecteur du modificateur de jet de capacité pour ajouter les attributs ATKxxx
* Ajout d'une section répétable "Autres traits" dans l'onglet Capacités, sous la liste des jets de capacités. Elle peut être montrée ou cachée (état préservé d'un appel de la fiche à l'autre). Cette nouvelle liste peut typiquement être utilisée pour noter les différents avantages liées aux types de surhumains, ou bien les différents implants d'un personnage cyberpunk, etc... Cette section comporte un bouton avec un picto "bulle" qui murmure la description du trait au joueur dans le chat. 
* Réorganisation de l'onglet Equipement
* Ajout d'une section répétables "Autres ressources" avec saisie d'un nom et d'une valeur numérique. Elle peut servir à comptabiliser les points de Provisions, de Munitions ou de Transport en univers Post-Apo, ou le seuil de Cyberlose et la difficulté du test de résistance en univers Cyberpunk
* Ajout d'une section masquable pour les caractéristiques d'un véhicule, avec une liste répétable de jets liés, sur lesquels on peut indiquer à la fois des caractéristiques de personnage et des caractéristiques de véhicule comme modificateurs au jet
* Ajout d'un élément {{text}} dans le roll template (utilisé par les jets d'affichage des "Autres traits")
* Correction d'une typo dans la bulle d'aide du bonus divers à la DEX (DEX_BONUS)
* Nouvelle classe de bouton 'output' représentée par un picto de bulle d'aide (pour affichage des "Autres traits" dans le chat)
* Augmentation à 250 pixels de la hauteur allouée à l'élément {{desc}} d'un roll template
* Ajout d'une classe text pour affichage d'un élément {{text}} dans le roll template (police italique réduite, texte justifié sans limite de hauteur)

## v2.1 (2018-12-07)
* Ajout d'onglets
* Ajout du support des états préjudiciables Aveuglé, Etourdi, Immobilisé, Renversé, Surpris avec buffs aux statistiques de combat correspondantes
* Ajout d'une option "Explosif" dans le sélecteur du type de jet pour des jets ouverts / sans limite
* Ajout du d3 au selecteur des dés de dommages
* Ajout d'un groupe de dés de dommages "sans limite" (armes à feu)
* Ajout de deux options d'attaque sur la deuxième ligne : relance (reroll et reroll once) et seuil de relance (à indiquer sous la forme d'un seuil -- relance des 1 par défaut).
* Ajout d'un état "Poisse" consistant à lancer deux d20 et garder le moins bon
* Race est remplacé par famille sur la fiche

## v1.0 (2018-11-07)

Création de la feuille.
