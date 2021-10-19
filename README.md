# projet_redstone 
Pour différents projet en redstone les bases sont toujours utiles alors faisont un petit tour des bases
## sommaire
- [ ] porte et
- [ ] porte ou
- [ ] inverseur
- [ ] ou exclusif

### porte et
table de vérité 
A | B | S
--| - | --
0 | 0 | 0
0 | 1 | 0
1 | 0 | 0
1 | 1 | 1

*légende
- fils de redstone
- 0 torche de restone
- o block

schema en block | x | x | x | x | x
--------------- | - | - | - | - | ---
A | - | o |     |   |   |   |   |
|  |   | - | 0 | - | S
B | - | o |

Une porte qui ne s'active que si toutes les entrées sont actives.

### porte ou
table de vérité 
A | B | S
--| - | --
0 | 0 | 0
0 | 1 | 1
1 | 0 | 1
1 | 1 | 1

*légende
- fils de redstone
- 0 torche de restone
- block

schema en block | x | x | x | x | x
--------------- | - | - | - | - | ---
A | - | 0 |     |   |   |   |   |
|  |   | ╠ | - | - | S
B | - | 0 |

La première fonction à plusieurs entrées. Si au moins une des entrées est active, la sortie est active. C'est-à-dire que si toutes les entrées sont actives, la sortie le sera aussi. Ce dernier point fait la différence par rapport à une porte XOR, ou exclusif.

### inverseur (NOT]
table de vérité 
A | S
--|--
0 | 1
1 | 0

légende
- fils de redstone
- 0 torche de restone
- o block

schema en block | x | x | x | x | x
----------------| - | - | - | - | -
A | - | o | 0 | - | S

La porte NOT est la porte la plus simple. Elle agit uniquement en inversant le signal. Si en entrée le signal est actif, en sortie le signal sera inactif. Son principal usage est le pilotage des torches en redstone, qui requièrent un signal nul pour éclairer.

C'est une construction de base que l'on retrouvera en tant qu'élément dans nombre d'autres portes.
 
 ### porte ou exclusif (XOR)
 table de vérité 
A | B | S
--| - | --
0 | 0 | 0
0 | 1 | 1
1 | 0 | 1
1 | 1 | 0

légende
- fils de redstone
- 0 torche de restone
- o block

schema en block | x | x | x | x | x
--------------- | - | - | - | - | ---
A |-|-|o|0|-|
 | |-| |-| |-|
 | |o|0|-| |-|S
 | |-| |-| |-|
B |-|-|o|0|-|

La porte XOR est une dérivée de la porte OR. Elle fonctionne de façon similaire, mais renvoie un signal nul si les deux entrées sont actives en même temps. C'est à dire qu'il faut que les entrées soient différentes.

## fin de la presentation des bases
- [x] porte et
- [x] porte ou
- [x] inverseur
- [x] ou exclusif

maintenant qu'on a vus les bases un monde de posibilité s'ouvre a vous combiner tous ca avec des piston et vous aller devennir un as 
