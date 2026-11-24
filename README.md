# FPS x Poker
Prototype de mécanique hybride : un système de poker simplifié mixé avec un duel FPS
------
## Concept

Le joueur reçoit une main de poker. La combinaison obtenue détermine l'arme avec laquelle il affronte son adversaire dans un duel en arène.

## Boucle de jeu

1. Distribution d'une main de 5 cartes
2. Un tour d'échange : le joueur peut jeter jusqu'à 3 cartes
3. Évaluation de la main
4. Attribution d'une arme selon la combinaison
5. Duel contre l'adversaire dans une arène
6. Fin de manche, retour à l'étape 1

## Combinaisons et armes (prototype)

| Combinaison | Arme |
|---|---|
| Carte haute | Pistolet classique (glock 17) |
| Paire | Pistolet semi-automatique (Berreta M9) |
| Brelan | Fusil à pompe (winchester M1897) |
| Couleur | Arme blanche (pas d'idée pour l'instant) |
| Full | Fusil automatique (M16 - AR15) |

Les armes ont des profils différents (portée, cadence, dégâts) plutôt qu'une simple échelle de puissance, afin d'éviter qu'une combinaison rare écrase toutes les autres. Cependant, une M16 en comparaison à un glock 17 reste une arme avec plus de munitions et une cadence plus élevé.

## Périmètre du prototype

- Une seule arène
- Un seul adversaire IA, qui reçoit aussi une main et une arme
- Cinq catégories d'armes
- Interface de cartes minimale

## Choix technique imposé

- Moteur : Unreal Engine 5
- Langage : Blueprints uniquement

## Feuille de route

- [ ] Deck, cartes et distribution
- [ ] Évaluateur de mains
- [ ] Table des armes
- [ ] Personnage FPS et arène
- [ ] Phase d'échange
- [ ] Adversaire IA
- [ ] Boucle complète
