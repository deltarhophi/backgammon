# Tutoriel · coups-ouverture (doubles au premier coup, tavla) · 2026-11-14

Mode : tutoriel (demandé par l'étudiant)
Conditions : normales; séance étalée du 2026-11-14 (10 h 15) au 2026-11-16 (résumé); tablier réaffiché quatre fois à sa demande
Résultat : étape 1 erronée (6-6 joué au lieu de 3-3), étape 2 erronée, étape 3 réussie (6-6 trouvé d'avance, 5-5 juste, raison complétée), exemple final non réussi; résumé non fait
Entrée du journal : 2026-11-14 · Tutoriel · coups-ouverture (Semaine 1, séance 1)

Précisions données : au backgammon, l'ouverture ne peut pas être un double (un dé chacun); au tavla, le gagnant de l'ouverture relance ses deux dés.

## Question 1 (étape 1, 3-3)
Réponse : « 13/7(2) / 24/18(2) » puis « Ah non j ai joué 6-6 »
Verdict : erroné · lecture (huit déplacements; l'étudiant avait en tête 6-6); réponse 8/5(2) 6/3(2); séparément 24/18(2) 7e (−0,140), 13/7(2) 9e (−0,159)
## Question 2 (étape 2, 4-4)
Réponse : « 13/5(2) »
Verdict : erroné · concept (3e, −0,127; meilleur 24/20(2) 13/9(2) : ancre avancée + point 9)
## Question 3 (étape 3, 6-6 et 5-5)
Réponses : 6-6 « 24/18(2) 13/7(2) » (via Q1, 1er choix) · 5-5 « 13/3(2) Les pions arrières ne peuvent pas bouger »
Verdict : maîtrisé (raison complétée : point 19 tenu par gnubg)
## Question 4 (exemple final, 2-2)
Réponse : « 13/9(2) On prépare les constructions et la prime »
Verdict : erroné · concept (13e, −0,204; meilleur 13/11(2) 6/4(2)) : quatre déplacements pour un seul point
## Résumé de l'étudiant
« Je ne suis pas sûr, il va falloir y revenir » → conclusion donnée par Claude.

## Fiches

# Fiches · Tutoriel · coups-ouverture (doubles) · 2026-11-14

Demande : « ouvertures avec double. Tutoriel. » Au backgammon, l'ouverture ne peut pas être un double (un dé chacun, égalité relancée); au tavla, le gagnant de l'ouverture relance ses deux dés : un double est possible au premier coup. Le tutoriel porte sur les doubles joués depuis la position de départ.
Réserve : gnubg évalue selon les règles du backgammon (videau, backgammon à 3); au tavla, les écarts de valeur peuvent légèrement changer.
Plan : 1 un double = quatre déplacements = deux points (3-3) · 2 l'ancre avancée (4-4) · 3 les deux barres et le cas du 5-5 · 4 exemple final (2-2).
Vérifications (GNU Backgammon 1.07.001, 2 plis, prune off, movefilter 1 0 -1 0 0 / 2 0 20 0 1.0 / 2 1 -1 0 0; position de départ, set turn 1) :
- 1-1 : 8/7(2) 6/5(2) +0,306 · 24/22 6/5(2) +0,268 (−0,038)
- 2-2 : 13/11(2) 6/4(2) +0,322 · 24/22(2) 6/4(2) +0,263 (−0,059) · 13/9 6/4(2) +0,239 (−0,083)
- 3-3 : 8/5(2) 6/3(2) +0,347 · 24/21(2) 8/5(2) +0,290 (−0,057) · 24/21(2) 13/10(2) +0,287
- 4-4 : 24/20(2) 13/9(2) +0,445 · 24/20(2) 8/4(2) +0,322 (−0,123) · 13/5(2) +0,318 (−0,127)
- 5-5 : 13/3(2) +0,169 · 13/3 8/3(2) −0,019 (−0,188) · 13/8(4) −0,179 (−0,348)
- 6-6 : 24/18(2) 13/7(2) +0,562 · 24/18 13/7(3) +0,322 (−0,240) · 13/7(4) +0,147 (−0,415)

## Q1 (étape 1) · Avec 3-3 depuis le départ, quels deux points peux-tu faire? Écris le coup.
Réponse : 8/5(2) 6/3(2) (points 5 et 3), 1er choix. Erreurs : 8/5(2) seul plus 13/10(2) → un seul point.
## Q2 (étape 2) · Avec 4-4, gnubg hésite entre 24/20(2) 13/9(2), 24/20(2) 8/4(2) et 13/5(2). Lequel préfère-t-il, et pourquoi en une phrase?
Réponse : 24/20(2) 13/9(2) (+0,445) : ancre sur son point 5 et un point sur 9 (constructeur sûr), sans dégarnir le 8; 8/4(2) et 13/5(2) à −0,12.
## Q3 (étape 3) · Avec 6-6, quel coup? Et pourquoi 5-5 est-il un cas à part?
Réponse : 24/18(2) 13/7(2) (les deux barres, +0,562; 13/7(4) −0,415). 5-5 : les pions arrière ne peuvent pas bouger (24/19 bloqué par son point 6) et 8/3 ne fait qu'un point; 13/3(2) fait le point 3 avec les pions du 13.
## Q4 (exemple final) · Avec 2-2, écris ton coup complet et justifie.
Réponse : 13/11(2) 6/4(2) (+0,322) : point 4 et point 11. Alternatives : 24/22(2) 6/4(2) (−0,059).
Relecture : ok; questions dans l'ordre sans fuite (chaque correction ne cite que son propre double).
