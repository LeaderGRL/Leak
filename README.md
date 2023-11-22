# Leak

## IA Utility
## Fonctionnement
### Behavior Tree
- Traquer le joueur
- Chercher le joueur dans des cachettes
- Se déplacer
- Tendre des embuscades 
### IA Utility
#### Pourcentage d'apparition
- 0% pendant 1min puis 50% et augmentation de 5% toutes les 10min
- +25% si bruit fort
#### Pourcentage disparition
- +1% toutes les secondes
- +10% si joueur très proche du monstre
#### Habitude des cachettes
- Au début du jeu le monstre cherche dans une cachette 
- Plus le joueur progresse et plus monstre augment le nombre de cachette dans lequel il cherche.
- Au 2/3 du jeu le monstre fouille toutes les cachettes du type que le joueurs à le plus utitlisé ce qui le forcera a chagner son style de jeu.

### TODO
- Diagrame interaction Behavior tree et IA utility
- IA Utility: info du joueur, alterne entre traque du joueur et fuite toute les 10 sec. 

### Question
- Comment le joueur sait que le monstre le traque ? -> A décider environnement / bruit sonore(claquement).
- Le monstre voit le joueur se cacher ? -> Oui
- le monstre tend des embuscades ? -> Oui, simple: attend au coin d'un couloir.

