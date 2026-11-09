# Tutoriel · frapper-ou-construire · 2026-11-08

Mode : tutoriel
Conditions : normales
Résultat : étapes 1, 3 et 4 réussies (4 avec justification complétée), étape 2 reprise puis réussie; exemple final non réussi (solution montrée à sa demande)
Entrée du journal : 2026-11-08 · Tutoriel · frapper-ou-construire (Semaine 2, séance 1)

Plan annoncé : 1 repérer les pions frappables · 2 ce que la frappe coûte à l'adversaire · 3 risque et temps · 4 comparer frapper et construire · 5 exemple final seul.
Fil rouge : 0HPkATDgc/ABMA, 4-2 (ouverture adverse 2-1 : 13/11 6/5). Exemple final : 4HPhASjgc/ABMA, 4-2 (ouverture adverse 4-1 : 24/23 13/9).
Demandes en cours de route : réaffichage du plateau (étape 3); « que veut dire le point 5 ? » et « faire son point 5, c'est déposer un pion dessus ? » → numérotation de chaque côté, faire un point = au moins deux pions.

## Question 1 (étape 1)
Réponse de l'étudiant : « l'adversaire a 14 et 20 seuls. je peux frapper 20 avec 24/20. ça laisserait 20 seul. je ne peux atteindre 14. »
Confiance : non demandée
Verdict : maîtrisé
Commentaire : repérage complet et distances justes; il anticipe déjà le pion seul laissé sur 20.
Question défectueuse : non

## Question 2 (étape 2)
Réponse de l'étudiant : « point 20, il perd 5 cases. point 2, il perd 23 cases »
Confiance : non demandée
Verdict : erroné · concept
Commentaire : confond le chemin qui reste au pion adverse avec le chemin perdu. Réexpliqué avec le compte des points du moteur (164 → 184 après 24/20*).
Question défectueuse : non

## Question 2b (remplacement)
Réponse de l'étudiant : « 11 cases avant de sortir, 14 perdues »
Confiance : non demandée
Verdict : maîtrisé
Commentaire : distinction faite; la réponse pour le point 2 (2 cases) a été donnée ensuite.
Question défectueuse : non

## Question 3 (étape 3)
Réponse de l'étudiant : « 24, 20 et 11 vont avoir des pions seuls » puis, relancé sur le pourquoi : « il aura du mal pcq il doit d'abord sortir son pion captif. Il lui faut 1 à 5. S'il a 5 et 6, il pourrait atteindre le 11. s'il a double-5, il pourrait attiendre le 20. »
Confiance : non demandée
Verdict : maîtrisé
Commentaire : compte et idée de rentrée justes (6 bloqué par son point 6, exemple 6-5 juste). Sous-estime les tirs sur 20 (pions adverses à 1, 3 et 6 cases) : relève de compter-tirs, signalé sans le travailler.
Question défectueuse : non

## Question 4 (étape 4)
Réponse de l'étudiant : « le moteur préfère frapper pcq construire je gagne 6 places, frapper l'adversaire recule de 20 »
Confiance : non demandée
Verdict : incomplet
Commentaire : bon choix (24/20* 13/11 +0,147 contre 8/4 6/4 −0,083); justification à moitié juste : les deux coups avancent de 6, ce qui départage est le recul, le temps et le point 5 empêché.
Question défectueuse : non

## Question 5 (exemple final)
Réponse de l'étudiant (1re tentative) : « je joue 24/18 18/16. je frappe son 16. il doit absolument sortir du bar, donc mon 16 seul est inatteignable. même s'il a double-4; il ne peut peut passer par 8. »
Verdict : erroné · lecture (coup illégal : 24/18 demande un 6 avec 4-2)
Réponse de l'étudiant (2e tentative) : « je joue 6/2 et 8/6. le 2 devient à découvert. c'est un risque que je prend. »
Verdict : erroné · concept (= 8/2*, −0,241 selon gnubg; meilleur : 8/4 6/4 +0,001)
Suite : indice ou solution proposés; réponse « langue au chat » → solution montrée : la frappe sur 2 ne fait reculer que de 2 cases et expose un pion seul au fond du jan (pion adverse sur 1, rentrée avec un 2); faire le point 4 vaut plus.
Confiance : non demandée
Question défectueuse : non

## Résumé de l'étudiant (avant complément)
« frapper doit rapporter plus que construire. il doit faire reculer beaucoup l'adversaire. »
Complété par : le temps que la rentrée fait perdre, le risque pour ses propres pions seuls (et ce qu'ils perdraient), la valeur du point qu'on renonce à faire.

## Fiches

# Fiches · Tutoriel · frapper-ou-construire · 2026-11-08

Fil rouge : position 0HPkATDgc/ABMA, X (joueur) à jouer 4-2. L'adversaire a ouvert 2-1 : 13/11 6/5 (pions seuls sur les points 20 et 14 du joueur). Compte des points : X 167, O 164.
Exemple final : position 4HPhASjgc/ABMA, X à jouer 4-2. L'adversaire a ouvert 4-1 : 24/23 13/9 (pions seuls sur les points 1, 2 et 16 du joueur). Compte : X 167, O 162.
Vérifications (GNU Backgammon 1.07, 2 plis, sans élagage : set evaluation movefilter 1 0 -1 0 0 / 2 0 20 0 1.0 / 2 1 -1 0 0; new game, set turn 1, set board <ID>, set dice, hint 8) :
- 0HPkATDgc/ABMA 4-2 : 1. 24/20* 13/11 +0,147 (53,1 %) · 2. 24/22 24/20* +0,134 · 3. 24/20*/18 +0,113 · 4. 24/20* 8/6 +0,055 · 5. 24/20* 6/4 +0,037 · 6. 8/4 6/4 −0,083 (47,9 %) · 7. 13/11 13/9 −0,208.
- après 24/20* 13/11 : compte O 164 → 184 (+20).
- 0HPkATDgc/ABMA 3-1 : 1. 24/20* +0,113 · 2. 8/5 6/5 −0,011.
- 4HPhASjgc/ABMA 4-2 : 1. 8/4 6/4 +0,001 (50,0 %) · 2. 24/22 6/2* −0,146 (46,6 %) · 3. 24/20 13/11 −0,147 · 7. 13/11 6/2* −0,175.
- après 24/22 6/2* : compte O 162 → 164 (+2).

## Q1 · identifier (étape 1)
Question : Dans cette position, quels pions de l'adversaire sont seuls? Lesquels peux-tu frapper avec ton 4-2, et par quel mouvement?
Objectif : après cette question, je saurai si l'étudiant sait repérer les pions adverses seuls et ceux qu'un lancer donné peut atteindre · Notion : frapper-ou-construire
Réponse attendue : pions seuls sur ses points 20 et 14. Seul celui du 20 est frappable : 24/20* (le 4, depuis 24). Le 14 demanderait 10 depuis 24.
Erreurs probables : compter le 14 comme frappable (6+4 ou 4+2 mal compté) → compte des distances; ne voir que l'un des deux pions seuls → lecture du plateau; proposer 13/... vers 14 → sens de marche inversé.
Devinable? Non : il faut lire le plateau et compter les distances.
Juste pour ces données? Vérifié sur le plateau gnubg; aucune frappe sur 14 dans la liste des coups légaux de hint.
Modèle : type classique (repérer les tirs, bkgm.com) · Piège : aucun
Relecture : ok

## Q2 · interpréter (étape 2)
Question : Si tu frappes le pion adverse sur ton point 20, combien de cases perd-il? Et s'il s'agissait d'un pion adverse seul sur ton point 2, combien en perdrait-il?
Objectif : après cette question, je saurai si l'étudiant sait estimer le terrain que la frappe fait perdre selon l'endroit · Notion : frapper-ou-construire
Réponse attendue : 20 cases; 2 cases. Un pion adverse sur ton point p a encore 25−p cases à faire; frappé, il repart de la barre (25) : il perd p cases.
Erreurs probables : 5 au lieu de 20 → compte du point de vue de l'adversaire (son point 5) au lieu du recul; 23 pour le point 2 → confusion entre ce qui reste et ce qui est perdu.
Devinable? Non : il faut raisonner sur le sens de marche adverse.
Juste pour ces données? Vérifié par gnubg : +20 pour 24/20* dans le fil rouge (164 → 184), +2 pour 6/2* dans 4HPhASjgc/ABMA (162 → 164).
Modèle : compte des points, bkgm.com · Piège : aucun
Relecture : ok

## Q3 · prédire (étape 3)
Question : Après 24/20* 13/11, combien de tes pions sont seuls, et sur quels points? Pourquoi l'adversaire aura-t-il plus de mal que d'habitude à les frapper au prochain tour?
Objectif : après cette question, je saurai si l'étudiant sait évaluer le risque d'une frappe et le temps qu'elle fait perdre · Notion : frapper-ou-construire
Réponse attendue : 3 pions seuls : 24, 20, 11. L'adversaire doit d'abord rentrer son pion avec un de ses dés; il ne lui en reste qu'un pour frapper, et s'il ne rentre pas, il ne joue pas du tout.
Erreurs probables : oublier le pion resté sur 24 → lecture; « parce qu'il a un pion de moins » sans la rentrée → ne voit pas la perte de temps.
Devinable? Non : il faut compter après le coup et relier à la règle de rentrée.
Juste pour ces données? Départ X : 24×2, 13×5, 8×3, 6×5; après 24/20* 13/11 : 24×1, 20×1, 13×4, 11×1, 8×3, 6×5 → 3 pions seuls.
Modèle : type classique · Piège : aucun
Relecture : ok

## Q4 · comparer (étape 4)
Question : Tu hésites entre 24/20* 13/11 (frapper) et 8/4 6/4 (faire ton point 4). Lequel le moteur préfère-t-il, selon toi? Justifie en une phrase avec ce qu'on a vu.
Objectif : après cette question, je saurai si l'étudiant sait comparer une frappe et un coup de construction dans une position donnée · Notion : frapper-ou-construire
Réponse attendue : 24/20* 13/11 (+0,147) devant 8/4 6/4 (−0,083), écart 0,230; victoires 53,1 % contre 47,9 %. Justification : la frappe fait perdre 20 cases et un demi-tour à l'adversaire, et l'empêche de faire son point 5 avec ce pion.
Erreurs probables : 8/4 6/4 « parce qu'un point est plus sûr » → surestime la sécurité, sous-estime le recul et le temps.
Devinable? En partie (deux options). Compensé par : justification exigée.
Juste pour ces données? Vérifié par gnubg (voir en tête).
Modèle : réponse à l'ouverture 2-1 en « slot », position classique · Piège : aucun
Relecture : ok, compensé par : justification exigée

## Q5 · exemple final (étape 5)
Question : Nouvelle position (4HPhASjgc/ABMA, diagramme affiché) : l'adversaire a ouvert 4-1 en jouant 24/23 13/9. Tu as 4-2. Écris ton coup complet, dis s'il frappe ou non, et justifie en une ou deux phrases.
Objectif : après cette question, je saurai si l'étudiant sait décider seul entre frapper et construire dans une position nouvelle · Notion : frapper-ou-construire
Réponse attendue : 8/4 6/4 (+0,001), sans frapper. La seule frappe (sur 2, par 6/2*) ne fait reculer le pion adverse que de 2 cases, laisse un pion seul au fond de ton jan, exposé au pion adverse sur 1 et à la rentrée; faire le point 4 vaut plus. Meilleure frappe : 24/22 6/2* −0,146 (victoires 46,6 % contre 50,0 %).
Erreurs probables : 24/22 6/2* ou 13/11 6/2* « parce qu'il faut frapper » → applique la frappe sans peser le terrain gagné; frappe sur 16 → distance (8 non disponible).
Devinable? En partie : deux familles de coups. Compensé par : coup complet et justification exigés.
Juste pour ces données? Vérifié par gnubg (voir en tête); seule frappe possible sur 2.
Modèle : réponse classique au « split » 4-1 · Piège : aucun (décider fait partie de l'objectif annoncé au plan)
Relecture : ok, compensé par : coup complet et justification exigés

## Q2b · interpréter (remplacement de Q2, étape 2)
Contexte : réponse à Q2 « point 20, il perd 5 cases. point 2, il perd 23 cases » → confusion entre ce qui reste à faire et ce qui est perdu.
Question : Le pion adverse seul sur ton point 14 (celui que tu ne pouvais pas atteindre) : combien de cases lui reste-t-il à faire avant de sortir, et combien en perdrait-il s'il était frappé?
Objectif : après cette question, je saurai si l'étudiant distingue le chemin restant et le chemin perdu par une frappe · Notion : frapper-ou-construire
Réponse attendue : il lui reste 11 cases (25−14); frappé, il repart de 25 : il perd 14 cases.
Erreurs probables : 11 pour les deux → même confusion; 14 et 11 inversés → sens de marche.
Devinable? Non : il faut les deux calculs, dans le bon sens.
Juste pour ces données? Vérifié par gnubg : fil rouge avec 6-4, 24/14* → compte O 164 → 178 (+14).
Modèle : compte des points, bkgm.com · Piège : aucun
Relecture : ok

Vérification de la 2e tentative (gnubg 2 plis, sans élagage, hint 40) : 8/2* −0,241 (44,1 %), 9e choix.
