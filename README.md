## Dans quelle mesure faire confiance à autrui est-il bénéfique pour nous ?


### COLLANGE Clément 
### CASTERA Chloé 
### LAVAL Léo 
### AYATILLAH Youssef

Nicky Case a créer un jeu basé sur une théorie permettant de montrer le phénomène de confiance au sein d’une population. C'est ce jeu que nous allons modéliser pour tenter de répondre à la problématique.

Pour le jeu, vous êtes face à une machine et jouer en même temps qu'une autre personne. Vous avez un choix à faire qui est de mettre une pièce ou non dans la machine. Si vous mettez une pièce l'adversaire en reçoit 3 et vice versa. Vous pouvez chacun choisir de coopérer (mettre une pièce) ou bien de tricher (ne pas en mettre). Par exemple si les deux joueurs trichent, il vont chacun perdre une pièce, on aura donc un score de 0-0.

Si les deux coopèrent ils gagnent chacun deux pièces. 
Si un joueur triche et l'autre non, celui ayant coopérer va perdre une pièce alors que celui ayant triché en aura gagner deux.

Par conséquent on pourrait se dire que pour être sûr de ne jamais perdre il faudrait toujours tricher. C'est là que se trouve le dilemme car coopérer peut laisser les autres prendre l'avantage sur nous. Maintenant intéressons-nous a ce qui se passe si on y joue plusieurs fois. Nous allons jouer contre 5 adversaires aux profils différents et effectuer entre 3 et 7 rounds (sans savoir quel round est notre dernier).

Nous auront en jeu plusieurs types de personnes : Le tricheur, le radin, le copieur, le méfiant, l'alternant, l'aléatoire et le coopératif. Ces types de joueurs ont tous des caractéristiques différentes.

• Le **copieur**: il coopère au premier tour puis reproduis ce que vous avez fait au tour précédant

• Le **tricheur** : il triche toujours

• Le **coopératif** : il coopère toujours

• Le **radin** : il commence par coopérer mais si on triche une fois il triche jusqu’à la fin

• Le **méfiant** : il triche au premier tour puis reproduis ce que vous avez fait au tour précédant

• L'**alternant** : il commence par jouer puis altèrne a chaque tour entre triche et coopération

• L'**aléatoire** : Il commence par coopérer puis triche ou coopère aléatoirement

Ce que nous allons rajouter du jeu de base sera une dyamique d'échange entre les contients Chaque continent contiendra des pourcentages de types de joueurs spécifiques et un nombre de joueurs différent. Les flux de joueurs sera le plus réalise possible, basé sur des pourcentages de migrations réels. Nous ferons fluctuer les gains et pertes entre les parties, l'argent de départ, ainsi que le nombre de manche, le pourcentage de population que l'on va supprimer et que l'on va dupliquer. 

Pour compenser la différence d'argent entre un continent avec beaucoup de personnes (et donc des joueurs avec beaucoup d'argent vu qu'ils ont fait beaucoup de partiesClément ) et un continent avec peu de personnes (donc des joueurs avec moins d'argent), on pourrait dupliquer les personnes ayant le plus d'argent moyen par partie, et non les plus riches.

## Le 13/03: compte rendu première séance

Notre but va être de modéliser l’évolution du nombre de joueurs de chaque catégorie au cours du temps en fonction de 
différents critères. Pour s'eloigner du jeu de Nick Case nous allons creer de nouveaux types de joueurs et surtout nous 
allons modeliser les échanges entre différents continents a partir des probabilités les plus réalistes possible.

A l'aide du planisphère predefni en python nous créer une interface visuelle permettant de representer les échanges au cours du temps

Nous avons commencé la programmation en s'attaquant à:

- Le déroulement d'une partie entre deux joueurs

- Le déroulement d'un échange entre tous les joueurs d'un continent 

- La création d'un continent contenant les types souhaités

Nous avons effectué des recherches sur le taux de migration mondiale entre les continents pour tenter d'obtenir un modèle le plus réaliste possible.

Nous avons également cherché le nombre d'habitants par continents.

## Le 20/03: compte rendu deuxieme séance

Objectif de la séance: 

- Terminer les recherches pour les pourcentages de migrations entre pays

- Creer les continents grace aux informations collectées

- Mise a jour des évolutions de population: les 10% ayant le moins d'argent laissent place aux 10% les plus riches qui vont 
se dupliquer

- Mise en place du système d'échange entre les continents et stabilisation de la population apres les échanges

- Commencer a chercher comment fonctionne la carte prédéfinie en python

Compte rendu :

Durant cette séance nous avons réalisé le code permettant de mettre à jour les populations en supprimant les 10% les plus pauvre et en copiant les 10% les plus riches en gardant le pourcentage modifiable. De plus nous avons créer les continents en fonctions de la populations réelle de la terre avec un ratio de 1 pour 10 000 000. Nous avons également réfléchis et commencer la fonction qui va nous permettre de faire les echanges entre les continents.

## Le 27/03: compte rendu troisième séance

- Nous avons régler le problème concernant les échanges, pour rappel les gains en Asie etaient beaucoup plus faible qu'en Océanie par exemple du fait du nombre de parties beaucoup plus élevées. Nous avons résolu le problème en divisant le nombre de gains par le nombre de parties jouées par la personne.

- Nous avons créer les graphismes de nos différents types de joueurs puis nous les avons intégré a notres carte. Basemap nous semblant trop compliqué nous avons importé une image de planisphère via pygame.

- Nous avons posté sur github un shéma explicatif représentant un tour complet dans un continent.

- Nous avons continué a améliorer notre interface graphique pour qu'elle soit le plus compréhensible et esthétique possible.


## Le 03/04: compte rendu quatrième séance

-

-
