# Leak

## IA Utility
## Fonctionnement
### Behavior Tree
- Traquer le joueur
- Atttaquer le joueur
- Chercher le joueur dans des cachettes
- Se déplacer
- Tendre des embuscades 
#### Capteurs (Visuel / Sonore / Autres)
##### Sonore
- Movement du joueur (marche / course)
- Tire des armes
##### Visuel
- Lumière
- Cachette
- - fouille certaintes cachette aléatoirement 
- - Passe devant la cachette
##### Autre
- Raycast derrière la tête

### IA Utility
Gère le comportement de la créature en fonction des informations qu'elles disposent sur le joueur.
#### Pourcentage d'apparition
- 0% pendant 1min puis 50% et augmentation de 5% toutes les 10min
- +25% si bruit fort
#### Pourcentage disparition
- +1% toutes les secondes
- +10% si joueur très proche du monstre
#### Dégat infligé par le joueur
- Si le joueur inflige beaucoup de dégât alors le monstre fuie.
#### Habitude des cachettes
- Au début du jeu le monstre cherche dans une cachette 
- Plus le joueur progresse et plus monstre augment le nombre de cachette dans lequel il cherche.
- Au 2/3 du jeu le monstre fouille toutes les cachettes du type que le joueurs à le plus utitlisé ce qui le forcera a chagner son style de jeu.

### TODO
- IA Utility: info du joueur, alterne entre traque du joueur et fuite toute les 10 sec. 

### Question
- Comment le joueur sait que le monstre le traque ? -> A décider environnement / bruit sonore(claquement).
- Le monstre voit le joueur se cacher ? -> Oui
- le monstre tend des embuscades ? -> Oui, simple: attend au coin d'un couloir.

 