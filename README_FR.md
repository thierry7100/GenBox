#Générateur de boîtes
##Présentation

Pour abriter les divers montages faits au Fablab, les boîtes découpées au laser sont d'un usage fréquent. J'ai décidé de créer une extension Inkscape permettant de réaliser des boîtes de ofrme diverses, le tout dans un seule extension. Les boîtes crées se veulent plus décoratives, que des boites rectangulaires toutes simples.
Comme de plus j'aime bien les arrondis, les boîtes crées peuvent généralement avoir des coins arrondis (de 1 à 4 coins arrondis).
Il est également possible d'avoir des "cases" à l'intérieur de la boîte, on fixe au départ le nombre de colonnes et de rangées.
Un exemple de ce qui est possible de faire:
<center>![Genbox_1](https://user-images.githubusercontent.com/35993911/69336078-5920c380-0c5e-11ea-80a9-4cab35be853f.png)</center>
 
##Matériel 

Rien... Sauf du bois pour passer à la réalisation concrète. <br>
Utilisez du bois assez mince (3 ou 5mm max). J'ai personnellement utilisé du MDF ou du contreplaqué peuplier.
Le MDF supporte bien le Flex, le contreplaqué un peu moins bien, les trais de coupe doivent être en effet dans le sens du bois, difficile avec du contreplaqué où les couches sont à 90°!. Mais c'est quand même possible, attention à la casse toutefois !

## Type de boîtes réalisables 

Voici quelques images de boîtes réalisées avec cette extension. La liste n'est pas exhaustive, le programme se veut générique et vous pouvez largement combiner les possibilités.
###Coins arrondis
Chaque coin peut être arrondi avec un rayon de courbure différent. Un rayon de courbure à 0 donne un coin droit. Attention, il n'est pas forcément possible de descendre en dessous de 10mm, le bois n'est pas si flexible !<br>
Les 4 coins peuvent être arrondis, ici avec le même rayon de courbure. Ici j'ai choisi, un couvercle simple<br>

<center>![Boite_Arrondie_01](https://user-images.githubusercontent.com/35993911/69336379-abfa7b00-0c5e-11ea-9606-e3e4086e7419.JPG)</center><br>

Vous pouvez également avoir ce style de forme avec les coins opposés arrondis, toujours avec un couvercle simple, notez dans ce cas la présence de cases dans la boîte:<br>
<center>![SimpleTop_02](https://user-images.githubusercontent.com/35993911/69336476-e2d09100-0c5e-11ea-808a-8c8685298e87.JPG)</center><br>
<center>Boîte avec couvercle posé</center><br>

### Type de couvercle

L'extension propose 7 types de couvercle
1. Sans couvercle : pas de dessus pour la boîte, pas d'encoches sur le haut
2. Boîte fermée : le dessus s'emboîte avec des encoches comme les autres faces. Solide, mais pas forcément facile à démonter !
3. Couvercle posé : le couvercle est obtenu en collant la pièce sans encoche qui englobe la boîte et l'intérieur découpé avec encoches. Cela permet au couvercle de tenir, tout en s'enlevant facilement. C'est ce qui est montré dans la seconde image ci-dessus.
4. Couvercle glissant : Le couvercle glisse sur le dessus de la boite. Des encoches sur les côtés permettent de retenir le couvercle et de le manipuler facilement. Voir exemple ci dessous. Attention dans ce cas, la boîte finie est un peu plus haute (2 fois l'épaisseur du bois) pour accueillir le système de glissière.
5. Couvercle avec charnière bois : Ici la boîte est surmontée de petites "oreilles" jouant le rôle de charnière. Tout est en bois, avec du MDF cela fonctionne très bien. Avec du contreplaqué, c'est également possible, mais cela coulisse un peu moins bien et fait un peu de bruit lors des ouvertures et fermetures. Voir également l'exemple ci-dessous. Le couvercle peut pivoter jusqu'à 180°, il repose dans cas sur la face arrière. 
6. Couvercle charnière métal : Les charnières sont constituées de petits morceaux de bois tournant autour d'un axe en métal. Je réalise cet axe à partir d'un clou (2.3 ou 2.4mm de diamètre) coupé à la bonne dimension avec une pince coupante. Le couvercle peut également pivoter à 180°. Voir photo ci dessous.
7. Couvercle style coffre : Ce couvercle utilise le même type de charnière que le précédent, mais le haut est bombé, comme dans un coffre ! Ce type de couvercle est incompatible avec des coins arrondis. <br>
<center>![Sliding_01](https://user-images.githubusercontent.com/35993911/69336551-07c50400-0c5f-11ea-8036-f1e671141f3a.JPG)]</center><br>
<center>Boîte avec couvercle coulissant</center><br>

<center>![IWood_01](https://user-images.githubusercontent.com/35993911/69336588-1f9c8800-0c5f-11ea-9f2a-caf73890aaf0.JPG)</center><br>
<center>Couvercle avec charnière bois</center><br>

<center>![Charniere_Metal_02](https://user-images.githubusercontent.com/35993911/69336628-3cd15680-0c5f-11ea-8421-768f504c6fbc.JPG)</center><br>
<center>Couvercle avec charnière métallique</center><br>

<center>![Coffre_01](https://user-images.githubusercontent.com/35993911/69336646-48bd1880-0c5f-11ea-8007-b010bed4a853.JPG) ![Coffre_02](https://user-images.githubusercontent.com/35993911/69336728-7904b700-0c5f-11ea-9aa4-79ae264ea779.JPG)</center><br>
<center>Couvercle type coffre</center><br>

##Le Logiciel

Il prend la forme d'un plugin inkscape. <br>
Pour l'installer, décompresser le .zip. Copier un des deux fichiers .inx (gen.box.inx si vous préférez l'interface en anglais, gen_box_fr.inx pour une interface en français) plus deux fichier .py qui contiennent le code.  Copiez les 3 fichiers (un interface, extension.inx, et les deux programmes, extension .py) dans le répertoire d'extension inkscape. Pour connaître celui-ci, la commande Edition/Préférences vous indique le chemin, soit du répertoire global, soit celui pour vous seul utilisateur. Sous Linux c'est ~/.config/inkscape/extensions pour le répertoire local que j'utilise. Sous Windows,c'est dans C:\Users\Votre Nom Utilisateur\AppData\Roaming\inskscape\extensions.  <br>
Voir ci dessous pour le mode d'emploi.

###Mode d'emploi

La partie interface homme-machine de l'extension se présente sous forme d'onglets
Les onglets sont a priori à utiliser dans l'ordre, qui se veut logique...

1. Onglet dimensions. Il donne les dimensions <bold>intérieures</bold> de la boîte. Vous pouvez choisir l'unité, mais seuls les mm ont été testés ! Bien faire attention à l'épaisseur du matériau sinon les encoches ne vont pas bien s'assembler. J'ai eu des matériaux qui ne respectent pas vraiment leurs côtes (ex MDF 3mm qui fait 3.2mm). Cela parait anodin, mais cela gêne considérablement voire empêche l'assemblage. L'entrée compensation du faisceau laser donne la "taille" de ca qui est enlevé par la laser. Pour du bois, 0.1mm est une bonne valeur. Pour du plexiglas ou du PMMA, monter à environ 0.2mm sinon les assemblages seront lâches et nécessiteront de la colle.<br>

<center>
![Onglet_Dimensions](https://user-images.githubusercontent.com/35993911/69336761-8fab0e00-0c5f-11ea-916b-4c8cdd9ac8fb.png)
</center><br>

2. Onglet coins arrondis. La permière case permet de forcer tous les coins comme droits. Sinon, vous pouvez choisir le rayon de courbure de chaque coin de manière indépendante. 0 indique un coin droit. Attention à ne pas mettre de valeur trop faible. Toute valeur supérieure à 0 et inférieure à 10 (environ) devrait être proscrite. <br>

Quand les 4 coins sont arrondis, il y a une bande unique pour le côté, elle peut donc être assez longue et dépasser la taille de la découpeuse laser. Il y a donc une option permettant de diviser en 2 cette bande. Ne pas utiliser cette opton si ce n'est pas nécessaire, cela ajoute des clips sur la face avant de votre boîte.

<center>![Onglet_CoinsArrondis](https://user-images.githubusercontent.com/35993911/69336767-93d72b80-0c5f-11ea-9c42-00ed50379fef.png)</center><br>

3. Onglet style de couvercle. Les différents styles de couvercle ont été détaillés dans le paragraphe précédent. Choisissez celui va convient à votre usage. Attention les couvercles à glissière ou avec charnière sont incompatibles avec des coins arrondis à l'arrière de la boîte. Pour les coffres, les 4 coins doivent être droits.
<center>
![Onglet_Couvercle](https://user-images.githubusercontent.com/35993911/69336771-976ab280-0c5f-11ea-92d0-d22e4161d1c7.png)</center><br>

4. Onglet cases intérieures. L'intérieur de la boîte peut être divisé en cases, vous pouvez fixer le nombre de colonnes et de rangées. Attention quand un de ces nombres un plus grand que 1, le logiciel génère une plaque intérieure, pour éviter d'avoir les encoches sur les faces visibles. Ne vous étonnez pas si vous avez un peu plus de pièces. La taille des cases doit être au minimum de 20mm, à vous de respecter cela.<br>

<center>
![OngletCasesInterieures](https://user-images.githubusercontent.com/35993911/69336801-a6e9fb80-0c5f-11ea-9f6f-d8ce6b19e5ce.png)</center><br>

5. Onglet encoches. Vous pouvez donner la taille des encoches par direction (X=longueur, Y= largeur, Z=hauteur). Vous pouvez aussi laisser l'extension choisir ce qui est raisonnable vu la taille de la boîte.<br>

<center>![OngletEncoches](https://user-images.githubusercontent.com/35993911/69336791-a3567480-0c5f-11ea-90db-360ee66d64c1.png)
</center><br>

## Évolutions possibles

A vous de me dire, ou à faire vous même...
Dans ce cas, n'oubliez pas de republier !

##Bilbiographie

Je me suis inspiré du site de Florian Festi, très bien fait, mais j'ai essayé de regrouper en une seule extension, et j'ai également corrigé quelques problèmes sur les boîtes générées.
Le site de FLorian Festi: [https://www.festi.info/boxes.py Festi.info]


