# Approfondir · frapper-ou-construire · 2026-11-08

Mode : approfondissement
Conditions : normales
Résultat : prérequis juste; cas d'application résolu avec le meilleur coup du moteur, justification juste
Entrée du journal : 2026-11-08 · Approfondir · frapper-ou-construire

Point de départ : analyse du 2026-11-08 (ww493535), deux frappes manquées (5-3 : bar/22 13/8 au lieu de bar/20* 13/10*, −1,220; 6-5 : 24/13 au lieu de 7/1* 6/1, −0,296).

Explication donnée : frapper fait perdre à l'adversaire du terrain (26 cases dans la position 5-3, vérifié par gnubg) et du temps (rentrée obligatoire, jeu bloqué tant qu'il n'est pas rentré); construire paraît plus sûr, d'où l'erreur; repère : chercher d'abord un pion adverse seul à portée, puis comparer la meilleure frappe au meilleur coup sans frappe; lien avec construire-points (frapper en faisant un point) et mise en garde (une frappe qui défait un point peut coûter cher).

## Question 0 (prérequis)

Question : Au backgammon comme au tavla, quand un de tes pions est frappé, que doit-il faire, et que se passe-t-il pour tes autres pions tant qu'il ne l'a pas fait?
Notion : frapper-ou-construire (prérequis : règles)
Réponse de l'étudiant : « il doit repasser par le jan 19-24. les autres pions ne peuvent bouger tant que ce n'est pas fait. »
Confiance : non demandée
Verdict : maîtrisé (prérequis)
Commentaire : règle complète : rentrée dans le jan adverse, reste du jeu bloqué.
Question défectueuse : non

## Question 1 (application)

Question : Tu as 4-4 et un pion à la barre. Tu rentres forcément avec bar/21. Il te reste trois 4 à jouer. Écris ton coup complet en notation, puis dis en une phrase pourquoi. (Position ID 0OfIQQKYZ/ABQg, partie contre aquavision, 3e coup)
Notion : frapper-ou-construire
Réponse de l'étudiant : « bar/21 13/9 9/5 13/9 » puis « 13/9 9/5 frappe un adversaire. le deuxième 13/9 me laisse à découvert, mais ça semble être le moins pire coup. »
Confiance : non demandée
Verdict : juste (= bar/21 13/5* 13/9, 1er choix de gnubg 2 plis); ne compte pas comme réussite (mode approfondir)
Commentaire : frappe repérée et chemin 13/9/5* trouvé; dans la partie réelle, il avait joué bar/21 8/4(2) 6/2 (−0,552). Le second 13/9 reconnu comme exposé; gnubg le préfère tout de même à 13/5*/1 (−0,069).
Question défectueuse : non

## Fiches

# Fiches · Approfondir · frapper-ou-construire · 2026-11-08

## Q0 (prérequis)
Question : Au backgammon comme au tavla, quand un de tes pions est frappé, que doit-il faire, et que se passe-t-il pour tes autres pions tant qu'il ne l'a pas fait?
Objectif : après cette question, je saurai si l'étudiant sait énoncer la règle de la frappe et de la rentrée · Notion : frapper-ou-construire (prérequis : règles)
Réponse attendue : il va sur la barre et doit rentrer dans le jan de l'adversaire (sur un point libre, selon un dé); tant qu'il n'est pas rentré, aucun autre pion ne peut bouger.
Erreurs probables : « il recommence au départ » sans la contrainte de rentrée → ignore que la rentrée bloque le reste du jeu (cœur du coût en temps de la frappe).
Devinable? Non : il faut connaître la règle de la rentrée obligatoire.
Juste pour ces données? Règle standard, identique au tavla (bkgm.com).
Modèle : règles de base, bkgm.com · Piège : aucun
Relecture : ok

## Q1 (application)
Position : partie contre aquavision (parties/2026-11-08-galaxy-50384696-aquavision.mat), ton 3e coup, gnubg coup 6 · Position ID 0OfIQQKYZ/ABQg · dés 4-4 · tu as un pion à la barre.
Question : Tu as 4-4 et un pion à la barre. Tu rentres forcément avec bar/21. Il te reste trois 4 à jouer. Écris ton coup complet en notation, puis dis en une phrase pourquoi.
Objectif : après cette question, je saurai si l'étudiant sait repérer une frappe disponible et la préférer à un coup de construction dans une position de début de partie · Notion : frapper-ou-construire
Réponse attendue : bar/21 13/5* 13/9 (gnubg 2 plis, éq. +0,296 en partie libre; +0,374 dans le contexte du match, export d'analyse). Toute frappe sur 5 est bien meilleure que son coup joué (bar/21 8/4(2) 6/2, −0,466 / −0,552). 2e : bar/21 13/5*/1 (−0,069). Non-frappe la meilleure : bar/21 13/9(3) (−0,089 à −0,104). Justification : le pion adverse seul sur ton point 5 est frappable avec deux 4 venant de 13 (13/9/5*); la frappe l'oblige à rentrer et lui fait perdre du temps, gammons 22 % contre 9 % pour le coup joué.
Erreurs probables : rejouer 8/4(2) 6/2 ou un autre coup de construction → ne voit pas la frappe ou la sous-estime; frappe impossible proposée (sur 7 ou 20 avec des 4) → lecture du plateau.
Devinable? En partie : la séance porte sur la frappe. Compensé par : coup complet exigé (il faut trouver le chemin 13/9/5*) et justification.
Juste pour ces données? Vérifié par GNU Backgammon 1.07, 2 plis : set board 0OfIQQKYZ/ABQg, set dice 4 4, hint. Seule frappe possible : sur 5 (7 et 20 inatteignables avec des 4).
Modèle : position tirée de la partie du joueur (regles-jeux.md, section 4) · Piège : aucun
Relecture : ok, compensé par : coup complet et justification exigés

## Vérifications pour l'explication
- Position 0HPMEwDgt8EBRA, 5-3 : après bar/20* 13/10*, compte des points X 144, O 168 (avant : X 152, O 142) → l'adversaire recule de 26 cases. gnubg : set board, set turn 1, set dice 5 3, move bar/20 13/10, show pipcount.
