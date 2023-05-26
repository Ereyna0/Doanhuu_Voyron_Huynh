# Doanhuu_Voyron_Huynh

Les commandes pour y jouer:

Pour jouer à notre jeu, il faut tout d’abord entrer le nombre de joueurs (de 2 à 4).

Après avoir entré le nombre de joueurs nous allons devoir créer les aventuriers qui vont explorer le labyrinthe. La création du joueur se fait par la fonction "creat_player(...)".

Pour créer les aventuriers vous devez tout d’abord inscrire votre nom, puis saisir la classe de l’aventurier ( magicien, guerrier, voleur ou archer).

Ensuite la partie peut commencer, nous vous rappelons que pour gagner l’aventurier doit trouver son arme légendaire associée ainsi qu’un coffre.
1. (le guerrier cherche l’épée de feu)
2. (le magicien cherche le grimoire légendaire)
3. (le voleur cherche la dague du sommeil)
4. (l’archer cherche l’arc légendaire)

Nous avons décidé de raisonner avec des switch / case pour gérer les interactions, donc les différentes cases que le joueur révèle au fur et à mesure. Voici la légende pour les cartes :
0 : ce sont les murs, donc la limite du plateau où le joueur ne peut y accéder.
3 : le portail
4 : les totems de transmutation. 
5 : les coffres
6 : l'épée de feu
7 : l'arc légendaire 
8 : la dague de sommeil
9 : le grimoire légendaire
10 : les Basilics
11 : les Zombies
12 : les Trolls
13 : les Harpies

L'intérêt d'attribuer ces légendes est de pouvoir remplir le labyrinthe de manière aléatoire avec le bon nombre d'éléments en effet il faut: 1 portail, 1 totem de transmutation, 2 coffres, 1 l’épée de feu, 1 arc légendaire, 1 dague de sommeil, 1 grimoire légendaire 4 basilics, 4 zombies, 4 trolls, 4 harpies. Pour rendre plus agréable l'expérience utilisateur, nous avons rajouté un affichemap3 qui se charge de l'interface graphique. 



Pour se déplacer dans le labyrinthe le joueur doit choisir entre 4 valeurs:
8 pour aller vers le haut
2 pour aller vers le bas 
4 pour aller vers la gauche
6 pour aller vers la droite

On ne peut de déplacer que vers des cases considérer comme non révélé
Pour équiper une arme afin de battre les monstres du le labyrinthe le joueur doit choisir entre 4 valeurs:
la valeur 1 pour le bouclier
la valeur 2 pour la torche
la valeur 3 pour la hache
la valeur 4 pour l’arc

On rappelle que:
le bouclier permet de battre le basilic, 
la torche  permet de battre le zombie,
la hache permet de battre le troll,
l’arc permet de battre la harpie


Dans le labyrinthe il existe des items:
- le portail qui permet de se téléporter dans le labyrinthe dans une case non révélée.
- le totem qui permet d’échanger la valeur dans la case dans le labyrinthe.Il permet d’échanger le totem avec une autre case du labyrinthe. Par exemple cela va intervertir le totem avec un monstre

