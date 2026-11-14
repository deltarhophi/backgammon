# Tutoriel · prime-et-ancre (bâtir une prime) · 2026-11-13

Mode : tutoriel
Conditions : normales; interrompu après l'étape 2 (l'étudiant est allé jouer)
Résultat : étapes 1 et 2 faites; étapes 3 et 4 (exemple final) non faites
Entrée du journal : 2026-11-13 · Tutoriel · prime-et-ancre (Semaine 2, séance 1)

Plan annoncé : 1 lire une prime et compter les sorties · 2 ne pas casser sa prime · 3 préparer l'allongement · 4 exemple final seul.
Position : xs7IATDYbuABMA (séquence légale, voir la préparation).

## Question 1 (étape 1)
Réponse de l'étudiant : « 4 points de suite » puis, relancé : « Il peut avec 1 et 2.  Ensuite peut-être un 5 peut passer, sinon il lui faut un 6. »
Verdict : incomplet (compte juste; raisonnement juste, lancers 6-1, 6-2, 5-2 et 6/36 complétés)
Question défectueuse : non

## Question 2 (étape 2)
Réponse de l'étudiant : « 13/8 6/5.  On ne casse pas notre prime, compare à 7/6. »
Verdict : maîtrisé (= 1er choix de gnubg; 13/8 7/6 −0,543)
Question défectueuse : non

## Question 3 (étape 3)
Posée (5-4 : classer 13/9 13/8, 13/4, 7/2 6/2), non répondue : séance interrompue.

## Question 4 (exemple final)
Non posée.
# Fiches · Tutoriel · prime-et-ancre (bâtir une prime) · 2026-11-13

Demande : « milieu de partie tutoriel », puis choix 1 (bâtir une prime), partie de prime-et-ancre non couverte au tutoriel du 2026-11-12.
Plan annoncé : 1 lire une prime et compter les sorties · 2 ne pas casser sa prime · 3 préparer l'allongement · 4 exemple final seul.

Position (construite par une séquence légale) : départ; toi 3-1 8/5 6/5; gnubg 5-2 13/8 13/11; toi 6-1 13/7 8/7; gnubg 6-4 8/2 6/2; toi 4-2 8/4 6/4; gnubg 3-1 8/5 6/5. Toi à jouer.
board simple 0 -2 0 0 2 2 3 2 0 0 0 0 -3 4 -1 0 0 -2 0 -3 -2 0 0 -2 2 0 · Position ID xs7IATDYbuABMA · compte toi 150, gnubg 146.
Vérifications (GNU Backgammon 1.07.001, 2 plis, prune off, movefilter 1 0 -1 0 0 / 2 0 20 0 1.0 / 2 1 -1 0 0) :
- Sorties d'un pion de gnubg sur ton point 1 derrière tes points 4-7 (énumération) : 6-1, 6-2, 5-2 = 6 lancers sur 36.
- 5-1 : 1. 13/8 6/5 +0,482 · 2. 13/7 +0,470 · 3. 13/8 7/6 −0,061 (−0,543) · 4. 7/6 7/2 −0,130 (−0,611).
- 5-4 : 1. 13/9 13/8 +0,571 · 2. 13/4 +0,462 (−0,109) · 3. 13/8 6/2 +0,201 (−0,370) · 4. 7/2 6/2 +0,061 (−0,510).
- 5-2 : 1. 13/11 13/8 +0,589 · 2. 24/22 13/8 +0,521 (−0,068) · 3. 13/8 6/4 +0,445 (−0,144) · 4. 13/6 +0,430 (−0,159).

## Q1 · identifier (étape 1)
Question : Combien de points consécutifs as-tu devant les pions de gnubg sur ton point 1? Avec quels lancers un de ces pions peut-il passer de l'autre côté?
Réponse attendue : 4 (tes points 4, 5, 6, 7). Sorties : 6-1, 6-2, 5-2 (6 lancers sur 36).
Erreurs probables : compter 6 (inclure 8 ou 3) → lecture; oublier qu'il faut s'arrêter sur des cases libres (6-6, 5-5 bloqués).
Devinable? Non. · Juste? Énumération (voir en tête). · Relecture : ok

## Q2 · comparer (étape 2)
Question : Tu as 5-1. Tu hésites entre 13/8 6/5 et 13/8 7/6. Lequel gnubg préfère-t-il, et pourquoi en une phrase?
Réponse attendue : 13/8 6/5 (+0,482) : le 1 se joue avec le pion de trop du 6, la prime reste entière; 13/8 7/6 casse ta barre et ouvre la sortie (−0,543).
Erreurs probables : 13/8 7/6 → ne voit pas qu'il casse le point 7.
Devinable? En partie. Compensé par : justification exigée. · Juste? gnubg. · Relecture : ok

## Q3 · prédire (étape 3)
Question : Tu as 5-4. Trois idées : 13/9 13/8, 13/4, 7/2 6/2. Classe-les et dis en une phrase ce que fait le meilleur pour la suite.
Réponse attendue : 13/9 13/8 (+0,571), 13/4 (+0,462), 7/2 6/2 (+0,061). Le meilleur place deux constructeurs juste au-dessus de ta prime, prêts à faire le 8 et allonger la prime.
Erreurs probables : 7/2 6/2 → fait un point au fond en cassant la prime.
Devinable? En partie. Compensé par : justification exigée. · Juste? gnubg. · Relecture : ok

## Q4 · exemple final
Question : Même position, tu as 5-2. Écris ton coup complet et justifie.
Réponse attendue : 13/11 13/8 (+0,589) : deux constructeurs au-dessus de la prime, sans la toucher. 13/8 6/4 (−0,144) empile; 13/6 (−0,159) n'ajoute rien devant.
Erreurs probables : 13/8 6/4 ou 13/6.
Devinable? En partie (même idée que Q3). Compensé par : coup complet exigé. · Juste? gnubg. · Relecture : ok, compensé par : coup complet exigé

## Reprise · 2026-11-13, 23 h 08 (après la fin du match)

## Question 3 (étape 3)
Réponse de l'étudiant : « 13/9 13/8  c'est une base pour construire ,mais 8 est vulnérable / 13/4  4 était déjà fait / 7/2 6/2  7 devient vulnérable »
Verdict : maîtrisé (ordre identique à gnubg)
Commentaire : nuance ajoutée : le constructeur sur 8 n'est atteignable que par des pions qui ont d'abord franchi la prime.
Question défectueuse : non

## Question 4 (exemple final)
Réponse de l'étudiant : « 13/8 24/22 je commence à travailler ma prime et je commence à sortir mes pièces arrières »
Verdict : incomplet (2e choix de gnubg, +0,521 contre +0,589 pour 13/11 13/8, −0,068)
Commentaire : un constructeur placé; le second (13/11) double les lancers qui font le point 8.
Question défectueuse : non

## Résumé de l'étudiant (avant complément)
« on n'essaie de ne pas empiler plus de deux pions par point.  on n'essaie de ne pas défaire la prime. »
Complété par : des points consécutifs; compter les sorties de l'adversaire; placer deux constructeurs juste au-dessus de la prime (8 à 11), peu exposés tant que l'adversaire est derrière; un pion de trop sert de rechange pour jouer sans casser.
