# Analyse · 2026-11-13-gnubg-2241-gnubg-complet.sgf · 2026-11-14

Mode : analyse de partie
Conditions : normales
Résultat : indice d'erreur global 36,3 mEMG (pions 39,7 · videau 16,5) sur le match (4 manches, 102 coups); match gagné 8-4
Entrée du journal : 2026-11-14 · Analyse · 2026-11-13-gnubg-2241-gnubg-complet.sgf

## Commande

```
python3 -I moteurs/backgammon_analyse.py parties/2026-11-13-gnubg-2241-gnubg-complet.sgf phili --plis 2
```

GNU Backgammon 1.07.001, 2 plis (pions et videau), seuil 0,020. Manches 2 à 4 extraites avec lire_decisions sur analyse_002.txt à analyse_004.txt.

## Estimation du joueur (avant l'analyse)

« je ne m'en souviens pas... d'ailleurs je n'ai pas compris comment s'est terminé la manche 2. »

Recoupement : aucun moment nommé; 0 des 4 erreurs retenues vue.

## Sortie du script

```
# Analyse gnubg · 2026-11-13-gnubg-2241-gnubg-complet.sgf · joueur : phili
Évaluation : 2 plis (pions et videau) · seuil des décisions listées : 0.020
Export complet : /tmp/gnubg-h23kc92m/analyse.txt

## Taux d'erreur (mEMG par décision, plus près de 0 = mieux)
- Pions : -39.7
- Videau : -16.5
- Global : -36.3
- Coups joués : 102

## Décisions coûteuses (3)
| Manche | Coup | Dés | Genre | Joué | Meilleur (gnubg) | Action correcte au videau | Perte |
|---|---|---|---|---|---|---|---|
| 1 | 12 | 41 | pions · very bad move | 18/14 6/5 | 6/2 5/4 |  | -0.931 |
| 1 | 8 | 43 | pions · doubtful move | bar/18 | bar/22 11/7 |  | -0.044 |
| 1 | 14 |  | videau · wrong take | accepts |  | Double, pass | -0.021 |
```

## Décisions coûteuses, manches 2 à 4 (extraction complémentaire)

```
export/analyse_002.txt
4 51 pions · bad move | 24/23 13/8 | 21/16 6/5 | No double, take (16.2%) -0.061
8 64 pions · doubtful move | bar/21* 11/5* | bar/21* 9/3 | No double, take (15.9%) -0.045
export/analyse_003.txt
31 63 pions · very bad move | 6/off 3/off | 6/3 6/off | Too good to double, pass (22.1%) -0.615
19 31 pions · very bad move | 13/10 4/3 | 10/9 4/1* | Too good to double, pass (36.6%) -0.26
17 43 pions · very bad move | 14/10 13/10 | 14/10 4/1* | Too good to double, pass (36.4%) -0.239
21 53 pions · very bad move | 10/5 6/3 | 10/7 6/1* | Too good to double, pass (36.6%) -0.232
5 42 videau · missed double | 8/4* 6/4 | 8/4* 6/4 | Double, pass -0.184
9 61 pions · doubtful move | 13/6 | 13/7 6/5 | Too good to double, pass (34.2%) -0.053
export/analyse_004.txt
6 22 pions · very bad move | bar/23(2) 7/5(2) | bar/23(2) 6/4(2) |  -0.12
8 54 pions · bad move | 6/1* 5/1 | 23/14 |  -0.102
2 33 pions · bad move | 13/7(2) | 24/21(2) 13/10(2) |  -0.072
4 51 pions · doubtful move | 24/23 13/8 | 24/18 |  -0.037
```

Chance (stats gnubg, match) : gnubg −2,549 EMG (−43,3 % de chances de match); phili +1,604 EMG (+32,4 %). Notes gnubg : jeu de pions « Awful! », videau « Intermediate ».

## Erreurs retenues

### 1. Ancre cassée face aux constructeurs adverses (prime-et-ancre)
Manche 1, coup 12, 41 · Position ID ss3BYQBw38DBAA · Match ID cAnmAAAAAAAE
Joué : 18/14 6/5 · gnubg : 6/2 5/4 · perte −0,931
Explication : tes deux pions sur le point 7 de gnubg (ton 18) tiennent un point dans son jeu; 18/14 le défait et laisse deux pions seuls (18 et 14) devant ses constructeurs. 6/2 5/4 joue dans ton jan sans rien exposer. Compte presque égal (134 contre 129) : pas de raison de partir.

### 2. Sortir en laissant un tir (sortie-sans-contact)
Manche 3, coup 31, 63 · Position ID 2L4LASDuZgAAAA · Match ID cAnvAEAAIAAE
Joué : 6/off 3/off · gnubg : 6/3 6/off · perte −0,615
Explication : gnubg a encore un pion sur ton point 1. 6/off 3/off laisse un pion seul sur 6, à 5 cases de lui. 6/3 6/off vide ton point 6 et ne laisse aucun pion seul. Avec un pion adverse derrière, la sécurité passe avant le nombre de pions sortis.

### 3. Frapper un deuxième pion pour gagner double (valeur-gammon)
Manche 3, coups 17, 19, 21 (43, 31, 53) · Position ID (coup 19) 4OfgAVC222EEAA
Joués : 14/10 13/10, 13/10 4/3, 10/5 6/3 · gnubg : 14/10 4/1*, 10/9 4/1*, 10/7 6/1* · pertes −0,239, −0,260, −0,232
Explication : gnubg a un pion sur la barre et un autre seul sur ton point 1; ta position est trop bonne pour doubler (gnubg passerait). Frapper le second pion met deux pions sur la barre face à ton jan presque fermé : les chances de gagner double (gammon) montent. Tu as joué à chaque fois un coup tranquille.

### 4. Double manqué (quand-doubler)
Manche 3, coup 5, 42 · Position ID 4OfgAQWMt8HBAA · Match ID cAnqAEAAIAAE
Joué : pas de double, 8/4* 6/4 · gnubg : doubler (gnubg aurait refusé), puis 8/4* 6/4 · perte −0,184
Explication : à 4-4 dans un match en 7, après ta frappe et tes points, ta position valait plus qu'un point : gnubg juge qu'il fallait doubler, et qu'il aurait abandonné la manche (1 point pour toi). Tu as gagné 2 points ensuite, mais la décision, au moment où elle a été prise, coûtait en moyenne.

## Positions (export gnubg)

```
Move number 12:  phili to play 41

 GNU Backgammon  Position ID: ss3BYQBw38DBAA
                 Match ID   : cAnmAAAAAAAE
 +13-14-15-16-17-18------19-20-21-22-23-24-+     O: gnubg
 | X           O  X |   | O  O  O     O    |     0 points
 | X           O  X |   | O  O  O          |     
 | X           O    |   |                  |     
 |                  |   |                  |     
 |                  |   |                  |    
v|                  |BAR|                  |     7 points match (Cube: 1)
 |                  |   | X                |    
 |                  |   | X                |     
 | O                |   | X  X             |     
 | O           O  X |   | X  X             |     Rolled 41
 | O           O  X |   | X  X             |     0 points
 +12-11-10--9--8--7-------6--5--4--3--2--1-+     X: phili
Pip counts: O 129, X 134

* phili moves 18/14 6/5

Proper cube action: No double, take (25.7%)
     1. Cubeful 2-ply    6/2 5/4                      Eq.: -0.069
     2. Cubeful 2-ply    7/3 5/4                      Eq.: -0.078 (-0.009)
     3. Cubeful 2-ply    6/5 6/2                      Eq.: -0.099 (-0.030)
     4. Cubeful 2-ply    7/3 6/5                      Eq.: -0.102 (-0.033)
     5. Cubeful 2-ply    7/2                          Eq.: -0.105 (-0.036)
*   13. Cubeful 2-ply    18/14 6/5                    Eq.: -1.000 (-0.931)

Move number 31:  phili to play 63

 GNU Backgammon  Position ID: 2L4LASDuZgAAAA
                 Match ID   : cAnvAEAAIAAE
 +13-14-15-16-17-18------19-20-21-22-23-24-+     O: gnubg
 | O           O  O |   | O  O  O          |     4 points
 |                O |   | O  O  O          |     
 |                O |   | O                |     
 |                  |   | O                |     
 |                  |   | O                |    
v|                  |BAR|                  |     7 points match (Cube: 1)
 |                  |   |                  | X  
 |                  |   |                  | X   
 |                  |   |          X  X    | X   
 |                  |   | X     X  X  X    | X   Rolled 63
 |                  |   | X     X  X  X  O | X   4 points
 +12-11-10--9--8--7-------6--5--4--3--2--1-+     X: phili
Pip counts: O 113, X 35

* phili moves 6/off 3/off

Proper cube action: Too good to double, pass (22.1%)
     1. Cubeful 2-ply    6/3 6/off                    Eq.: +1.618
*    2. Cubeful 2-ply    6/off 3/off                  Eq.: +1.003 (-0.615)
     3. Cubeful 0-ply    6/off 4/1*                   Eq.: +0.158 (-1.460)

Move number 19:  phili to play 31

 GNU Backgammon  Position ID: 4OfgAVC222EEAA
                 Match ID   : cInlAEAAIAAE
 +13-14-15-16-17-18------19-20-21-22-23-24-+     O: gnubg
 | X           O    | O | O                |     4 points
 |             O    |   | O                |     
 |             O    |   | O                |     
 |                  |   | O                |     
 |                  |   | 6                |    
v|                  |BAR|                  |     7 points match (Cube: 1)
 |                  |   |                  |    
 | O                |   |                  |     
 | O                |   | X     X          |     
 | O     X          |   | X  X  X  X  X    |     Rolled 31
 | O     X          |   | X  X  X  X  X  O |     4 points
 +12-11-10--9--8--7-------6--5--4--3--2--1-+     X: phili
Pip counts: O 161, X 83

* phili moves 13/10 4/3

Proper cube action: Too good to double, pass (36.6%)
     1. Cubeful 2-ply    10/9 4/1*                    Eq.: +2.191
     2. Cubeful 2-ply    6/5 4/1*                     Eq.: +2.167 (-0.024)
     3. Cubeful 2-ply    4/1* 2/1                     Eq.: +2.147 (-0.044)
     4. Cubeful 2-ply    10/9 10/7                    Eq.: +1.992 (-0.199)
     5. Cubeful 2-ply    10/7 6/5                     Eq.: +1.988 (-0.203)
*   10. Cubeful 2-ply    13/10 4/3                    Eq.: +1.931 (-0.260)

Move number 17:  phili to play 43

 GNU Backgammon  Position ID: 4OfgAVC22wELAA
                 Match ID   : cAnuAEAAIAAE
 +13-14-15-16-17-18------19-20-21-22-23-24-+     O: gnubg
 | X  X        O    | O | O                |     4 points
 | X           O    |   | O                |     
 |             O    |   | O                |     
 |                  |   | O                |     
 |                  |   | 6                |    
v|                  |BAR|                  |     7 points match (Cube: 1)
 |                  |   |                  |    
 | O                |   |                  |     
 | O                |   | X     X          |     
 | O                |   | X  X  X  X  X    |     Rolled 43
 | O                |   | X  X  X  X  X  O |     4 points
 +12-11-10--9--8--7-------6--5--4--3--2--1-+     X: phili
Pip counts: O 161, X 90

* phili moves 14/10 13/10

Proper cube action: Too good to double, pass (36.4%)
     1. Cubeful 2-ply    14/10 4/1*                   Eq.: +2.159
     2. Cubeful 2-ply    13/9 4/1*                    Eq.: +2.149 (-0.010)
     3. Cubeful 2-ply    5/1* 4/1                     Eq.: +2.116 (-0.043)
     4. Cubeful 2-ply    6/2 4/1*                     Eq.: +2.081 (-0.078)
     5. Cubeful 2-ply    14/7                         Eq.: +1.960 (-0.199)
*    8. Cubeful 2-ply    14/10 13/10                  Eq.: +1.920 (-0.239)

Move number 21:  phili to play 53

 GNU Backgammon  Position ID: 4OfgAVB22+EAAA
                 Match ID   : cInuAEAAIAAE
 +13-14-15-16-17-18------19-20-21-22-23-24-+     O: gnubg
 |             O    | O | O                |     4 points
 |             O    |   | O                |     
 |             O    |   | O                |     
 |                  |   | O                |     
 |                  |   | 6                |    
v|                  |BAR|                  |     7 points match (Cube: 1)
 |                  |   |                  |    
 | O                |   |                  |     
 | O     X          |   | X        X       |     
 | O     X          |   | X  X  X  X  X    |     Rolled 53
 | O     X          |   | X  X  X  X  X  O |     4 points
 +12-11-10--9--8--7-------6--5--4--3--2--1-+     X: phili
Pip counts: O 161, X 79

* phili moves 10/5 6/3

Proper cube action: Too good to double, pass (36.6%)
     1. Cubeful 2-ply    10/7 6/1*                    Eq.: +2.224
     2. Cubeful 2-ply    6/1* 4/1                     Eq.: +2.123 (-0.101)
     3. Cubeful 2-ply    10/7 10/5                    Eq.: +2.069 (-0.155)
     4. Cubeful 2-ply    10/2                         Eq.: +1.994 (-0.230)
*    5. Cubeful 2-ply    10/5 6/3                     Eq.: +1.992 (-0.232)

Move number 5:  phili to play 42

 GNU Backgammon  Position ID: 4OfgAQWMt8HBAA
                 Match ID   : cAnqAEAAIAAE
 +13-14-15-16-17-18------19-20-21-22-23-24-+     O: gnubg
 | X           O  X |   | O                |     4 points
 | X           O  X |   | O                |     
 | X           O    |   | O                |     
 |                  |   | O                |     
 |                  |   | 6                |    
v|                  |BAR|                  |     7 points match (Cube: 1)
 |                  |   |                  |    
 | O                |   | X                |     
 | O                |   | X                |     
 | O           X  X |   | X        X       |     Rolled 42
 | O           X  X |   | X  O  O  X       |     4 points
 +12-11-10--9--8--7-------6--5--4--3--2--1-+     X: phili
Pip counts: O 153, X 135

* phili moves 8/4* 6/4
Alert: missed double (-0.184)!
Proper cube action: Double, pass
*    1. Cubeful 2-ply    8/4* 6/4                     Eq.: +0.869
     2. Cubeful 2-ply    13/7                         Eq.: +0.725 (-0.144)
     3. Cubeful 2-ply    8/4* 7/5*                    Eq.: +0.641 (-0.228)
     4. Cubeful 2-ply    13/9 6/4*                    Eq.: +0.570 (-0.299)
     5. Cubeful 0-ply    8/6 8/4*                     Eq.: +0.531 (-0.338)```

## Le reste
9 autres décisions coûteuses, de −0,021 à −0,120, dont une acceptation de double à refuser (manche 1, −0,021).
