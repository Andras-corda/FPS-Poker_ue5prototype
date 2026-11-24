# FPS x Poker
Hybrid mechanic prototype: a simplified poker system mixed with an FPS duel
------
## Concept

The player is dealt a poker hand. The resulting combination determines the weapon used to face the opponent in an arena duel.

## Game Loop

1. Deal a 5-card hand
2. One exchange round: the player can discard up to 3 cards
3. Hand evaluation
4. Weapon assignment based on the combination
5. Duel against the opponent in an arena
6. End of round, back to step 1

## Combinations and Weapons (prototype)

| Combination | Weapon |
|---|---|
| High card | Classic pistol (Glock 17) |
| Pair | Semi-automatic pistol (Beretta M9) |
| Three of a kind | Shotgun (Winchester M1897) |
| Flush | Melee weapon (no idea yet) |
| Full house | Automatic rifle (M16 - AR15) |

Weapons have different profiles (range, fire rate, damage) rather than a simple power scale, to prevent a rare combination from overpowering all the others. That said, an M16 compared to a Glock 17 still has more ammo and a higher fire rate.

## Prototype Scope

- A single arena
- A single AI opponent, who also receives a hand and a weapon
- Five weapon categories
- Minimal card interface

## Imposed Technical Choices

- Engine: Unreal Engine 5
- Language: Blueprints only

## Roadmap

- [ ] Deck, cards and dealing
- [ ] Hand evaluator
- [ ] Weapon table
- [ ] FPS character and arena
- [ ] Exchange phase
- [ ] AI opponent
- [ ] Full loop
