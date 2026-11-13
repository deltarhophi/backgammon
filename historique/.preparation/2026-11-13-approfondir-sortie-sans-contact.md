Abandonné le 2026-11-13 (l'étudiant a préféré travailler la sortie des pions arrière avant de répondre au prérequis)
# Fiches · Approfondir · sortie-sans-contact · 2026-11-13

Point de départ : analyse du 2026-11-13 (match du 2026-11-12, 23 h 21), manche 3, 1-1 : 4/1 3/2 au lieu de 5/4 3/off, aucun pion sorti, course 33 contre 32, −0,220. Position ID cg4AANQLAAAAAA.
Mode : approfondir (une erreur précise et récente, type concept; notion jamais travaillée).

Position des questions 1 et 2 (board simple 0 0 1 2 2 2 2 0 0 0 0 0 0 0 0 0 0 0 0 -2 -2 -2 -2 -2 -1 0) : toi 2×1, 3×2, 4×2, 5×2, 6×2 (9 pions, 6 sortis), compte 38; gnubg 11 pions dans son jan (4 sortis), compte 41. Aucun contact.

Vérifications (GNU Backgammon 1.07.001, 2 plis, prune off, movefilter 1 0 -1 0 0 / 2 0 20 0 1.0 / 2 1 -1 0 0; hint 60) :
- 3-2 : 1. 3/off 2/off +0,742 (2 pions sortis) · 2. 5/off +0,657 · 3. 3/1 3/off +0,654 · 8. 6/1 +0,563 · 9. 5/2 3/1 +0,522 (−0,220, aucun pion sorti).
- 1-1 : 1. 3/off 2/1 +0,543 · 2. 4/off +0,533 · 3. 5/4 3/off +0,529 · 8. 5/1 +0,425 (−0,118, premier coup sans sortie) · 11. 6/2 +0,397.

## Q0 · prérequis
Question : Tous tes pions sont dans ton jan, et le plus haut est sur ton point 4. Tu fais un 6. Que peux-tu faire avec ce 6?
Objectif : après cette question, je saurai si l'étudiant connaît la règle de sortie avec un dé plus grand · Notion : sortie-sans-contact (prérequis)
Réponse attendue : sortir un pion du point 4 (un dé plus grand que le pion le plus haut sort ce pion).
Erreurs probables : « rien » → ignore la règle du dé supérieur.
Devinable? Non.
Juste pour ces données? Règle standard (bkgm.com).
Modèle : règles de base · Piège : aucun
Relecture : ok

## Q1 · application (3-2)
Question : (position ci-dessus) Course pure, aucun contact. Tu as 3-2. Écris ton coup et combien de pions il sort.
Objectif : après cette question, je saurai si l'étudiant cherche d'abord à sortir le plus de pions · Notion : sortie-sans-contact
Réponse attendue : 3/off 2/off, deux pions sortis (+0,742). 5/2 3/1 n'en sort aucun (−0,220).
Erreurs probables : 5/off ou 3/1 3/off → un seul pion; 5/2 3/1 → déplace sans sortir.
Devinable? En partie. Compensé par : coup et nombre de pions exigés.
Juste pour ces données? Vérifié par gnubg.
Modèle : sortie de base · Piège : aucun
Relecture : ok, compensé par : coup et nombre exigés

## Q2 · application (1-1)
Question : (même position) Tu as 1-1, soit quatre 1 à jouer. Écris ton coup et combien de pions il sort.
Objectif : après cette question, je saurai si l'étudiant sait utiliser un petit double pour sortir un pion · Notion : sortie-sans-contact
Réponse attendue : un coup qui sort un pion : 3/off 2/1 (+0,543), 4/off ou 5/4 3/off (à 0,014 près). Sans sortie : 5/1 (−0,118), 6/2 (−0,146).
Erreurs probables : 5/1 ou 6/2 → « aucun pion ne peut sortir avec un 1 » sans voir qu'un pion du 3 ou du 4 sort avec trois ou quatre 1.
Devinable? Non : il faut voir qu'un pion peut utiliser plusieurs 1.
Juste pour ces données? Vérifié par gnubg.
Modèle : même motif que l'erreur du joueur · Piège : aucun
Relecture : ok
