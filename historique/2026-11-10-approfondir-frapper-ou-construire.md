# Approfondir · frapper-ou-construire · 2026-11-10

Mode : approfondissement
Conditions : normales
Résultat : prérequis juste; deux cas d'application résolus avec le premier choix du moteur, justifications justes (la première complétée)
Entrée du journal : 2026-11-10 · Approfondir · frapper-ou-construire

Point de départ : tutoriel du 2026-11-08 (exemple final non réussi : frappe sur 2 qui rapporte peu) et analyses du 2026-11-09 (frappes faibles sur le point 4; frappes manquées « frapper et faire le point » 63 et 55; frappe manquée avec 36 points de retard, 44).
Confusion nommée : frappe là où ça rapporte peu, manque les frappes qui rapportent beaucoup.
Explication donnée : trois questions avant de frapper : combien de cases il perd (p sur ton point p); ce que je laisse derrière (risque d'une frappe en retour, chère au fond de son jan); puis-je frapper et couvrir; erreur tentante : une frappe paraît active où qu'elle soit; lien avec compte-des-points (derrière dans la course, chaque frappe compte double).

## Question 0 (prérequis)
Question : Un pion adverse seul est sur ton point 9. Si tu le frappes, combien de cases perd-il? Et s'il était sur ton point 3?
Notion : frapper-ou-construire (prérequis)
Réponse de l'étudiant : « 9 : recul de 9 cases / 3: recul de 3 cases »
Confiance : non demandée
Verdict : maîtrisé (prérequis)
Commentaire : juste; la confusion du tutoriel (chemin restant contre chemin perdu) n'est pas revenue. Justification non écrite.
Question défectueuse : non

## Question 1 (application, frapper et faire le point)
Question : (diagramme 4HPkQSDgc/ABMA) gnubg a ouvert 6-2 en jouant 24/18 13/11 : il a un pion seul sur ton point 7 et un sur ton point 14. Tu as 6-1. Écris ton coup complet, puis justifie en une ou deux phrases.
Notion : frapper-ou-construire
Réponse de l'étudiant : « 13/7, 8/7.  je frappe et je fait le point 7.  meilleur coup d'ouverture dans ce cas »
Confiance : non demandée
Verdict : juste (= 13/7* 8/7, 1er choix de gnubg); ne compte pas comme réussite (mode approfondir)
Commentaire : justification juste mais courte; complétée : 7 cases perdues et rentrée obligatoire, aucun pion seul laissé, le point 7 bloque ses 6.
Question défectueuse : non

## Question 2 (application, quel pion frapper)
Question : (diagramme 4HPhASjgc/ABMA) gnubg a ouvert 4-1 en jouant 24/23 13/9 : il a des pions seuls sur tes points 1, 2 et 16. Tu as 5-3. Écris ton coup complet, puis justifie en une ou deux phrases. Si tu frappes, dis pourquoi ce pion-là.
Notion : frapper-ou-construire
Réponse de l'étudiant : « je joue 24/16.  Il recule de 16 cases.  le reisque est que je laisse 16 à découvert, ainsi que 24 »
Confiance : non demandée
Verdict : juste (= 24/16*, 1er choix de gnubg); ne compte pas comme réussite (mode approfondir)
Commentaire : bon pion choisi et recul juste; risque nommé (pions seuls sur 16 et 24). Astérisque de frappe omis dans la notation.
Question défectueuse : non

## Fiches

# Fiches · Approfondir · frapper-ou-construire · 2026-11-10

Point de départ : tutoriel du 2026-11-08, exemple final non réussi (frappe sur 2 qui rapporte peu); analyses du 2026-11-09 (8 h 01 et 23 h 26) : frappes sur le point 4 qui rapportent peu, frappes manquées dont deux « frapper et faire le point » (63 : 10/4* 7/4; 55 : 13/3 9/4* 8/3) et une frappe manquée avec 36 points de retard (44 : 22/10* 22/18).
Mode choisi : approfondir (règle « encore flou ou non acquis à la fin d'une séance : un autre mode que le dernier ; tutoriel → approfondir sur l'étape non réussie »).

Vérifications (GNU Backgammon 1.07.001, 2 plis, prune off, movefilter 1 0 -1 0 0 / 2 0 20 0 1.0 / 2 1 -1 0 0; set player 0/1 human; new game; set turn 1; set board simple …; set dice; hint 8) :
- 4HPkQSDgc/ABMA (gnubg a ouvert 6-2 : 24/18 13/11), 6-1 : 1. 13/7* 8/7 +0,105 · 2. 24/23 13/7* −0,046 (−0,150) · 3. 13/7*/6 −0,085 · 4. 24/18 8/7* −0,085 · 5. 13/7* 6/5 −0,127.
  Compte après 13/7* 8/7 : O 159 → 166 (+7); après 24/23 13/7* : O 159 → 166 (+7).
- 4HPhASjgc/ABMA (gnubg a ouvert 4-1 : 24/23 13/9; position de l'exemple final du tutoriel du 2026-11-08, autre lancer), 5-3 : 1. 24/16* +0,167 · 2. 8/3 6/3 −0,090 (−0,257) · 3. 24/21 13/8 −0,116 · 4. 24/21 6/1* −0,124 (−0,291) · 6. 13/10 6/1* −0,177.
  Compte après 24/16* : O 162 → 178 (+16); après 6/1* 24/21 : O 162 → 163 (+1).

## Q0 · prérequis
Question : Un pion adverse seul est sur ton point 9. Si tu le frappes, combien de cases perd-il? Et s'il était sur ton point 3?
Objectif : après cette question, je saurai si l'étudiant sait calculer le terrain qu'une frappe fait perdre selon l'endroit · Notion : frapper-ou-construire (prérequis)
Réponse attendue : 9 cases; 3 cases. Un pion adverse sur ton point p repart de la barre : il perd p cases.
Erreurs probables : 16 et 22 → confond le chemin restant (25−p) avec le chemin perdu (erreur du tutoriel du 2026-11-08).
Devinable? Non : il faut la règle du recul.
Juste pour ces données? Règle vérifiée par gnubg dans le tutoriel du 2026-11-08 (+20 pour une frappe sur 20, +2 sur 2) et ci-dessus (+7, +16, +1).
Modèle : compte des points, bkgm.com · Piège : aucun
Relecture : ok

## Q1 · application (frapper et faire le point)
Question : (diagramme 4HPkQSDgc/ABMA) gnubg a ouvert 6-2 en jouant 24/18 13/11 : il a un pion seul sur ton point 7 et un sur ton point 14. Tu as 6-1. Écris ton coup complet, puis justifie en une ou deux phrases.
Objectif : après cette question, je saurai si l'étudiant sait reconnaître une frappe qui fait aussi un point et la préférer · Notion : frapper-ou-construire
Réponse attendue : 13/7* 8/7 (+0,105). Il frappe sur 7 (7 cases perdues, rentrée obligatoire) et fait le point 7 du même coup : aucun pion seul laissé sur 7, et le point 7 bloque ses 6 depuis ton point 1. 24/23 13/7* frappe aussi mais laisse un pion seul sur 7 (−0,150).
Erreurs probables : 24/23 13/7* ou 13/7*/6 → frappe sans couvrir; 24/18 13/12 ou un coup sans frappe → ne voit pas la frappe.
Devinable? En partie : la séance porte sur la frappe. Compensé par : coup complet et justification exigés (il faut trouver 8/7 pour couvrir).
Juste pour ces données? Vérifié par gnubg (voir en tête); seules frappes possibles sur 7 (14 hors de portée avec 6-1 depuis 24 : 10 cases).
Modèle : réponse classique à l'ouverture 6-2 (« point sur la tête ») · Piège : aucun
Relecture : ok, compensé par : coup complet et justification exigés

## Q2 · application (quel pion frapper)
Question : (diagramme 4HPhASjgc/ABMA) gnubg a ouvert 4-1 en jouant 24/23 13/9 : il a des pions seuls sur tes points 1, 2 et 16. Tu as 5-3. Écris ton coup complet, puis justifie en une ou deux phrases.
Objectif : après cette question, je saurai si l'étudiant sait choisir entre frapper un pion avancé, frapper un pion au fond et construire, selon le terrain que la frappe fait perdre · Notion : frapper-ou-construire
Réponse attendue : 24/16* (+0,167). Le pion sur ton point 16 a déjà avancé : frappé, il perd 16 cases (162 → 178), contre 1 pour une frappe sur ton point 1 (6/1*). Faire le point 3 (8/3 6/3, −0,257) vaut moins que ce recul.
Erreurs probables : 8/3 6/3 → construit par réflexe sans peser la frappe; 6/1* + autre → frappe le mauvais pion (1 case); 13/5 → ne voit pas la distance de 8 (5+3) depuis 24.
Devinable? En partie (trois familles de coups). Compensé par : coup complet et justification exigés (dire quel pion et pourquoi).
Juste pour ces données? Vérifié par gnubg (voir en tête); 24/16* est la seule frappe sur 16 (13 ne recule pas; 24−8 = 16).
Modèle : position de l'exemple final du tutoriel du 2026-11-08, autre lancer; type classique (frapper le pion avancé) · Piège : aucun
Relecture : ok, compensé par : coup complet et justification exigés
