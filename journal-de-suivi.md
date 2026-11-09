# Journal de suivi : Backgammon (Minerva-Jeux)

Joueur : Philippe · pseudo Backgammon Galaxy : deltarhophi
Jeu : backgammon · Variantes : backgammon (Backgammon Galaxy); tavla (en personne, sans fichier)
Moteur : GNU Backgammon · Fiche : moteurs/backgammon.md des skills jeu-*
Niveau de départ : débutant
Mode : réel
Brief du projet : https://claude.ai/artifact/KQGbQaBxBtJZMFwAdvE7pz
Détail des activités : voir le dossier `historique/`
Gabarit : journal-gabarit.md de Minerva, version dfb9ef6 (2026-10-26)

<!--
Minerva-Jeux : ce journal suit un jeu, pas un cours (règles complètes : regles-jeux.md des skills jeu-*).
- « Semaine » = bloc de priorité (1, 2, 3…); « Séance » = 1; le Calendrier reste vide. Pas de rappel, pas d'examen, pas de carte de l'examen.
- Aucune notion n'est masquée : il n'y a jamais de rappel à attendre. N'écris pas « sans rappel préalable ».
- Le moteur nommé dans l'en-tête tranche : toute position, tout meilleur coup, toute évaluation lui est soumis avant d'être posé ou affirmé.
- Une partie ne valide jamais une notion. Une notion citée dans « Erreurs » d'une entrée Analyse est erronée à cette date (règle Rouge).
- Quiz : pas de diagnostic; variantes après tutoriel ou approfondissement; espacé = mélange des blocs, positions tirées des parties du joueur puis positions nouvelles sur le même motif.
- Priorités : notions en cause dans les analyses récentes, puis le bloc le plus bas.
- Statut : utiliser jeu-faire-le-point, pas faire-le-point (qui masquerait les notions faute de dates).
-->

<!--
Mode d'emploi
- Ce fichier est la mémoire du système d'étude. Les skills le lisent pour choisir quoi travailler.
- On n'y fait que cinq opérations, toujours ciblées, jamais une réécriture du fichier entier :
  1. ajouter une entrée À LA FIN de la section « Entrées »;
  2. ajouter une ligne à la section « Notions du cours », quand une notion nouvelle apparaît;
  3. ajouter une ligne à la section « Calendrier », quand la date d'une séance devient connue;
  4. ajouter une ligne à la section « Notions retirées », quand une notion est scindée ou fusionnée;
  5. ajouter une ligne à la section « Synonymes », quand un autre terme désigne une notion existante.
- On ne modifie ni ne supprime jamais une ligne existante. Une correction devient une nouvelle entrée.
- Après chaque écriture, relis la fin du fichier pour vérifier que l'entrée est là et que les entrées précédentes n'ont pas disparu.
- « Mode » : `simulation` si le dossier du cours commence par `sim-` (voir `garde-fous.md`, section 10); sinon `réel`. Un cours ne change jamais de mode.
- « Date de départ » : écrite par `demarrer-cours` quand le cours est démarré en cours de session. Elle règle la mise à niveau de la matière antérieure (voir « Matière antérieure à la date de départ »).
- L'état des notions (couleurs) n'est JAMAIS enregistré ici : `faire-le-point` et `preparer-examen` le recalculent chaque fois à partir des entrées.
-->

## Notions du cours

Liste de référence, créée par `demarrer-cours` à partir du plan de cours. **Tous les skills désignent les notions par leur code**, dans les entrées et les fichiers d'historique.

### Ce qu'est une notion

Une notion est **ce que l'étudiant doit être capable de faire**, sous la forme d'un objectif observable : « être capable de calculer le SSR d'une droite donnée », et non « le SSR ». Le nom court sert à l'affichage; l'**objectif** fixe la frontière. Une notion passe quatre tests :

1. **Diagnostic** : on peut écrire une question dont l'échec pointe vers cette notion-là, pas vers une voisine.
2. **Taille** : 1 à 3 questions suffisent à la vérifier, et une séance `etudier-notion` à la travailler. S'il faut plus de 3 types de questions différents, scinde-la; si on ne peut pas écrire 2 questions différentes sur elle, fusionne-la avec une voisine.
3. **Indépendance** : on peut réussir l'une et ne pas réussir l'autre. Une notion qui en suppose une autre (calculer un résidu → calculer le SSR) reste distincte : c'est un prérequis, pas un doublon.
4. **Ancrage** : elle vient des objectifs d'apprentissage du cours, ou d'une question des anciens examens ou des exercices. Chaque question d'examen correspond à au moins une notion; chaque notion peut faire l'objet d'au moins une question de type examen.

Repère d'homogénéité : **3 à 6 notions par séance**. Moins de 2 ou plus de 8 signale un découpage douteux.

| Trop large | Bonne taille | Trop fine |
|---|---|---|
| Régression | Calculer le SSR d'une droite donnée | Signe d'un résidu |

### Le code : la clé unique de chaque notion

Chaque notion a un **code** : sa clé unique, que tous les skills utilisent dans les entrées et les fichiers d'historique. Le nom, lui, sert seulement à l'affichage.

- Format : minuscules, **sans accents**, mots séparés par des tirets, 1 à 5 mots : `avantage-comparatif`, `somme-carres-residus`, `regression`.
- Langue : codes et noms dans la langue de travail de l'étudiant (le français); les termes de la langue du cours (l'anglais, par exemple) vont dans les synonymes.
- Les noms aussi doivent être uniques, notions retirées comprises : une nouvelle notion ne reprend jamais le nom d'une ancienne.
- Lisible : le code dit ce qu'est la notion. Une faute de frappe se voit, et tombe presque toujours sur un code inexistant que `faire-le-point` détecte.
- Unique et définitif : un code ne change jamais et ne sert qu'à une notion, même retirée.

**Synonymes** : un autre terme qui désigne **exactement la même capacité** qu'une notion existante (abréviation, terme anglais du cours, ancienne formulation) ne crée pas une notion; il s'ajoute à la section « Synonymes », avec le code qu'il désigne. Un synonyme ne désigne qu'un seul code; si un synonyme a été mal associé, ajoute une nouvelle ligne pour le même terme : **la ligne la plus récente fait foi**.

- Un terme **plus large** (« régression » quand la liste a `somme-carres-residus` et `derivation-moindres-carres`) n'est jamais un synonyme : dans une entrée, cite chaque code concerné.
- Un terme **plus étroit** (« signe d'un résidu » pour `residu`) n'est pas un synonyme non plus : c'est une facette de la notion, qui ne suffit pas à la confirmer.

Les skills reconnaissent une notion par son code, ses synonymes ou son nom, comparés **sous forme normalisée** (sans majuscules, accents, apostrophes ni espaces : `SSR`, `ssr` et `S.S.R.` sont le même terme), mais **écrivent toujours le code**.

### Ajouter, scinder, fusionner

- **Avant tout ajout, fais le scan** : parcours les codes, les noms, les synonymes et surtout les **objectifs** de toutes les notions existantes, retirées comprises, sous forme normalisée, en particulier de la même semaine et des semaines voisines. Si l'objectif d'une notion existante couvre déjà le nouveau terme, ajoute un **synonyme**, pas une notion. Sinon, vérifie que la nouvelle notion passe les quatre tests.
- **Ajouter** : une ligne (code, semaine, séance, nom court, objectif), et signale-le dans l'entrée de l'activité (« Notion ajoutée : `code` »). Un synonyme ajouté se signale aussi (« Synonyme ajouté : ssr → `somme-carres-residus` »).
- **Scinder ou fusionner** : seulement quand une notion échoue clairement au test de taille, et après l'avoir proposé à l'étudiant. Ajoute les nouvelles notions dans la liste (avec des codes et des noms nouveaux), puis une ligne dans « Notions retirées » pour chaque ancienne notion, par son code, avec la date et les codes qui la remplacent. « Remplacée par » ne cite que des notions **créées pour l'occasion** : pour fusionner A dans B qui existait déjà, retire A **et** B, et crée une notion nouvelle; sinon B garderait des confirmations qui n'ont jamais vérifié A. Après le retrait, les entrées citent les nouveaux codes, jamais l'ancien. Les nouvelles notions **repartent de zéro** : une réussite sur « Régression » ne prouve pas qu'il sait dériver les estimateurs. Signale-le dans l'entrée de l'activité (« Notion scindée : … »).
- Ne crée jamais une deuxième notion pour un concept qui existe déjà, ne réutilise jamais un code, et ne modifie jamais une ligne existante.

Chaque notion est rattachée à la séance où elle est enseignée (`k` = 1 s'il n'y a qu'une séance cette semaine-là).

**Journal créé avant les codes** (tableau sans colonne Code) : le code d'une ancienne notion est son nom normalisé (« Coût d'opportunité » → `cout-d-opportunite`). Ne réécris pas l'ancien tableau : ajoute les nouvelles notions dans un second tableau, sous le premier, avec l'en-tête à colonne Code, sans répéter les anciennes.

<!-- une ligne par notion, par exemple : | avantage-comparatif | 2 | 1 | Avantage comparatif | déterminer quel pays a l'avantage comparatif à partir des coûts d'opportunité | -->
| Code | Semaine | Séance | Notion | Objectif (être capable de…) |
|---|---|---|---|---|
| coups-ouverture | 1 | 1 | Coups d'ouverture | jouer correctement les 15 lancers d'ouverture |
| compter-tirs | 1 | 1 | Compter les tirs | compter les lancers sur 36 qui touchent un pion seul à une distance donnée |
| risque-pion-seul | 1 | 1 | Risque du pion seul | choisir, entre deux coups, celui qui laisse le moins de tirs à l'adversaire |
| construire-points | 1 | 1 | Construire des points | donner la priorité aux points 5 et 4, puis au point 7 (la barre) |
| differences-tavla | 1 | 1 | Différences du tavla | dire ce que chacune des différences du tavla change dans une situation donnée : ouverture relancée, pas de videau, pas de backgammon, pas de frapper-et-repartir dans son jan, pas de gaspillage à la sortie |
| frapper-ou-construire | 2 | 1 | Frapper ou construire | décider entre frapper un pion adverse et construire un point |
| compte-des-points | 2 | 1 | Compte des points | faire le compte des points et dire si la course est favorable |
| prime-et-ancre | 2 | 1 | Prime et ancre | bâtir une prime et tenir une ancre dans le jan adverse |
| sortie-sans-contact | 2 | 1 | Sortie sans contact | sortir ses pions en fin de partie sans laisser de tir |
| accepter-refuser | 3 | 1 | Accepter ou refuser | accepter ou refuser un double selon la règle des 25 % |
| quand-doubler | 3 | 1 | Quand doubler | reconnaître une position où doubler est correct |
| valeur-gammon | 3 | 1 | Valeur du gammon | tenir compte du risque de gammon dans une décision |

## Notions retirées

Notions scindées ou fusionnées. Elles ne comptent plus dans le statut ni dans le SPI; leurs anciennes entrées restent dans le journal.

<!-- par exemple : | regression | 2026-11-03 | somme-carres-residus; derivation-moindres-carres | -->
| Code | Date | Remplacée par |
|---|---|---|

## Synonymes

Autres termes qui désignent une notion existante. Un synonyme ne désigne qu'un seul code.

<!-- par exemple : | SSR | somme-carres-residus | puis | sum of squared residuals | somme-carres-residus | -->
| Synonyme | Code |
|---|---|
| opening moves | coups-ouverture |
| pip count | compte-des-points |
| take or drop | accepter-refuser |

## Calendrier

Date de chaque séance, d'après le plan de cours ou confirmée par l'étudiant. **Ne déduis jamais une date** (à partir d'un jour de cours habituel, par exemple) : une semaine de relâche ou un congé décalerait tout. Une séance sans ligne ici a une date inconnue; demande-la à l'étudiant quand tu en as besoin, puis ajoute la ligne.

Une séance déplacée reçoit une nouvelle ligne avec la mention « déplacée »; la ligne la plus récente fait foi.

<!-- une ligne par séance, par exemple : | 4 | 1 | 2026-10-21 | plan de cours | -->
| Semaine | Séance | Date | Source |
|---|---|---|---|

## Vocabulaire commun

### Statuts d'une notion dans une activité

- **maîtrisé** : réponse juste (quiz, séance de révision, examen blanc). Avec la confiance « sûr », c'est une **réussite sûre**.
- **incomplet** : partiel, vague, réussi sans certitude (« hésitant » ou « au hasard »), ou idée juste sous une forme insuffisante.
- **erroné** : contient une erreur ou une confusion.
- **absent** : pas mentionné ou pas tenté.
- **présent et juste** : statut propre au **rappel**. La notion est apparue spontanément et sans erreur dans la page blanche. Le rappel sert à repérer les oublis et les erreurs, pas à valider : ce statut ne compte **jamais** comme une réussite.

### Couleurs d'une notion (calculées, jamais enregistrées)

Applique ces règles **dans l'ordre** ; la première qui s'applique donne la couleur.

1. **Gris** : aucune entrée ne mentionne la notion.
2. **Rouge** : au **dernier contact**, la notion était :
   - erronée ou absente (rappel, quiz, séance de révision, examen blanc), ou elle a coûté des points à un examen réel;
   - encore floue après un approfondissement ou une synthèse;
   - non réussie ou sautée : exemple final d'un tutoriel, carte d'application, ou notion non acquise en fin de mémorisation.
   - *Sauté* (non tenté) : rouge par prudence, mais affiché « · exemple final non tenté », et `etudier-notion` reprend **la même méthode** là où elle s'est arrêtée. Changer de méthode est réservé aux vraies erreurs.
   - *Exception* : un « absent » dans un **rappel global** ne rend pas rouge une notion qui a déjà au moins une réussite sûre; elle est alors jaune.
3. **Vert** : toutes ces conditions sont réunies :
   - au moins **deux réussites sûres**, à au moins deux jours d'intervalle;
   - au moins une de ces réussites dans une activité qui mélange plusieurs semaines (quiz espacé, séance de révision, examen blanc, examen réel);
   - le dernier contact **dans un quiz, une séance de révision, un examen blanc ou un examen réel** date de **14 jours ou moins**.
4. **Jaune** : tous les autres cas (réussie une seule fois, réussie sans certitude, présente et juste dans un rappel, réussie dans un mode de `etudier-notion` (mémoriser, approfondir, tutoriel, synthèse), verte mais pas revue depuis plus de 14 jours).

Ce qui compte comme **réussite sûre** : une réponse juste avec la confiance « sûr », notes fermées, dans un quiz, une séance de révision ou un examen blanc; ou une question d'un examen réel réussie. Ne comptent **jamais** : le rappel et les quatre modes de `etudier-notion` (mémoriser, approfondir, tutoriel, synthèse), parce que la réussite y suit l'explication de près. Une carte mémorisée devient une réussite sûre quand elle est retrouvée plus tard dans un quiz, notes fermées, avec « sûr ».

**Légende pour l'étudiant** (à reprendre mot pour mot) :

> 🟥 **à corriger** : erreur, oubli ou essai non tenté au dernier contact, ou encore floue après un travail sur la notion · ⬜ **pas encore travaillée** · 🟨 **fragile** : travaillée, pas encore validée deux fois · 🟩 **acquise** : réussie au moins deux fois avec certitude, à quelques jours d'intervalle, dont une fois dans un quiz mélangé, et revue depuis moins de deux semaines

Pour un cours avec une **date de départ**, ajoute sous la légende, mot pour mot : « Matière d'avant ton arrivée (semaines 1 à N−1) : une seule réussite suffit pour 🟩; la préparation au final donnera la deuxième. »

### Matière antérieure à la date de départ

Quand un cours est démarré en cours de session, la matière des semaines **antérieures à la semaine de départ** (en-tête « Date de départ ») suit une règle allégée, parce que la préparation à l'examen final (rappel global, séances de révision, examen blanc) fournira la deuxième exposition :

- **Vert** : **une** réussite sûre dans une activité qui mélange plusieurs semaines (un quiz de mise à niveau compte), et le dernier contact dans un quiz, une révision, un examen blanc ou un examen réel date de 14 jours ou moins. Les règles gris, rouge et jaune ne changent pas.
- **Mise à niveau** : `demarrer-cours` découpe cette matière en blocs d'**environ 8 notions**, dans l'ordre des semaines, un quiz espacé par bloc avec une question par notion, et l'annonce (« 4 quiz pour te mettre à niveau : semaines 1-2, 3-4, 5, 6 »). Une notion non réussie pendant la mise à niveau devient 🟥 et suit ensuite le parcours normal. Chaque quiz de mise à niveau porte « · mise à niveau » à la fin de son en-tête, par exemple `## 2026-10-28 · Quiz espacé · Semaines 1-2 · mise à niveau`.
- **Dates** : les séances antérieures n'ont pas besoin de date au Calendrier; elles n'attendent plus de rappel et ne sont jamais masquées.
- Les notions des semaines à partir de la semaine de départ suivent les règles normales.

### Unités d'effort (calculées, jamais enregistrées)

Une **unité** vaut environ 20 minutes de travail actif avec les skills. Elle se déduit du type de chaque entrée; ne l'écris jamais dans le journal.

| Entrée | Unités |
|---|---|
| Rappel (un rappel global : 1 par séance couverte, au plus 3 en tout) | 1 |
| Quiz (diagnostic, variantes, espacé; un quiz partiel aussi) | 1 |
| Approfondir | 1 |
| Mémoriser | 1 |
| Synthèse (une vérification de synthèse : 1) | 2 |
| Tutoriel | 2 |
| Séance de révision | 2 |
| Examen blanc | 1 par tranche de 20 minutes de sa durée prévue, arrondie au supérieur |
| Démarrage, Plan de révision, Copie corrigée | 0 |

Une séance `etudier-notion` qui enchaîne deux modes compte les deux entrées. Pour répartir les unités entre les parties de la matière, une entrée qui touche plusieurs semaines partage ses unités à parts égales entre elles.

Les unités mesurent l'**effort**, jamais la **maîtrise** : elles n'interviennent dans aucune règle de couleur. Elles ne couvrent pas non plus les lectures et les exercices faits hors des skills, qui forment la plus grande part du temps d'étude.

### SPI de maîtrise (calculé, jamais enregistré)

Le SPI (*schedule performance index*) dit si la maîtrise **confirmée** suit le rythme du cours. Il ne compte pas l'effort (ce sont les unités) : il compte des **confirmations**.

**Confirmation** : une réussite sûre sur une notion, obtenue dans un quiz, une séance de révision, un examen blanc ou un examen réel (copie corrigée). Chaque notion en demande deux :

- **C1** : une première réussite sûre;
- **C2** : une deuxième réussite sûre, à au moins 2 jours de l'autre, l'une des deux dans une activité qui mélange plusieurs semaines (quiz espacé, révision, examen blanc, examen réel).

Si le dernier résultat d'une notion dans une de ces activités est **erroné ou absent**, ses confirmations retombent à zéro; seules les réussites obtenues après cet échec comptent. Une entrée dont les conditions ne sont pas normales (notes consultées, rappel le jour même, écarts à l'examen blanc) ne donne aucune réussite, mais ses échecs comptent.

**Formule**, pour une notion *n* enseignée à la date *dₙ*, au jour *t* :

- confirmations prévues : PVₙ = 0 si t − dₙ < 4 jours; 1 si 4 ≤ t − dₙ < 14; 2 si t − dₙ ≥ 14;
- confirmations obtenues : EVₙ = 0, 1 ou 2, selon les règles ci-dessus;
- **s'il y a au moins une notion en retard** (EVₙ < PVₙ) : **SPI = Σ min(EVₙ, PVₙ) ÷ Σ PVₙ**. L'avance sur une notion ne compense jamais le retard d'une autre;
- **si aucune notion n'est en retard** : **SPI = (Σ PVₙ + avance) ÷ Σ PVₙ**, où l'avance = Σ max(EVₙ − PVₙ, 0);
- le SPI est arrondi **vers le bas** au centième, plafonné à **1,15**, et affiché seulement si Σ PVₙ ≥ 6.

**Règles prudentes** (une erreur doit faire baisser le SPI, jamais le gonfler) :

- dₙ vient du Calendrier; si la séance n'y est pas, dₙ = le lundi de sa semaine, déduit d'une date connue (la date la plus tôt possible);
- le SPI n'est **pas affiché** (« non fiable ») si une séance passée n'a aucune notion dans la liste; si une mention dans les entrées n'est ni un code, ni un nom, ni un synonyme; si un code apparaît deux fois; si une entrée cite un nom porté par deux notions; si une ligne de « Notions retirées » est incomplète ou cite un code absent; si un échec cite une notion après son retrait; si un synonyme pointe vers une notion retirée; ou si aucune date ne permet de situer une semaine;
- **matière antérieure à la date de départ** : PVₙ = 0 pendant les 14 jours qui suivent la date de départ, puis 1 (jamais 2); EVₙ = 1 si une réussite sûre dans une activité mélangée suit le dernier échec. Si le Calendrier est vide, la date de départ et sa semaine servent d'ancre pour dater les semaines suivantes;
- le SPI ne retire pas une confirmation à cause du temps écoulé : l'oubli se voit par la couleur (vert non revu depuis 14 jours → jaune), pas par le SPI.

Le calcul se fait par le script `scripts/spi.py` du skill `faire-le-point`, pas de tête.

**Pour que le calcul soit juste, écris les entrées exactement au format** : en-tête `## AAAA-MM-JJ · <type> · <objet>`, un champ par puce de premier niveau, les notions d'un champ sur la même ligne, séparées par des virgules, désignées par leur **code**.

### Autres termes

**Confiance** : sûr · hésitant · au hasard

**Types d'erreur** : vocabulaire · calcul · concept · lecture · forme · temps

**Non réussi** (code `non-reussi`, s'il faut un code) : remplace « raté » partout, dans le journal comme à l'affichage. **Sauté** : étape, carte ou exemple non tenté (voir la règle Rouge).

**Conditions** : normales · rappel le jour même · notes consultées · sans rappel préalable (modes de `etudier-notion` seulement)

**Séance** : identifiée par `Semaine N, séance k` (k = 1 s'il n'y a qu'une séance cette semaine-là).

## Formats d'entrée

Chaque skill écrit son entrée **exactement** dans le format ci-dessous. Toutes commencent par `## AAAA-MM-JJ · <type> · <objet>`. Partout où un format dit `<notions>` ou `<notion>`, écris les **codes** de « Notions du cours » (par exemple « Maîtrisé : avantage-comparatif, cout-opportunite »).

### Démarrage

```
## AAAA-MM-JJ · Démarrage · <cours>
- Structure créée : <liste>
- Plan de cours : <lu | manquant>
- Ressources à déposer : <exercices, anciens examens, copies corrigées>
- Mise à niveau : <blocs, par exemple « semaines 1-2, 3-4, 5-6 », ou « sans objet »>
```

### Rappel

```
## AAAA-MM-JJ · Rappel · Semaine N, séance k : <thème>
- Niveau : solide | partiel | fragile
- Estimation de l'étudiant : <ce qu'il pensait avoir oublié ou mal compris> · Réel : <ce que la correction a montré>
- Erroné : <notions>
- Absent : <notions>
- Incomplet : <notions>
- Présent et juste : <notions>
- Priorités : <au plus 3>
- Signaux de l'enseignant : <ou « aucun »>
- Quiz diagnostique prévu : <une date>
- Détail : historique/<fichier>.md | non conservé
```

Un **rappel global** fait pendant `preparer-examen` produit une entrée Rappel par séance couverte, avec `(rappel global)` à la fin de l'en-tête et « Quiz diagnostique prévu : sans objet (rappel global) ».

### Approfondir

```
## AAAA-MM-JJ · Approfondir · <notions>
- Conditions : <normales | sans rappel préalable>
- Approfondi : <notions>
- Encore flou : <notions, ou « rien »>
- Vérification : <faite | interrompue>
- Questions défectueuses : <ou « aucune »>
- Détail : historique/<fichier>.md | non conservé
```

### Mémoriser

```
## AAAA-MM-JJ · Mémoriser · <notions> (Semaine N, séance k)
- Conditions : <normales | sans rappel préalable>
- Cartes : <n> (dont 1 d'application)
- Acquises en séance : <notions dont toutes les cartes ont 3 réussites>
- Non acquises en fin de séance : <notions, ou « aucune »> (sa carte d'application n'est pas réussie, ou une de ses cartes est restée sous 3 réussites et sa dernière réponse est non réussie ou sautée)
- À revoir : <notions ni acquises ni non acquises, par exemple séance arrêtée, ou « rien »>
- Cartes sautées : <notions, ou « aucune »>
- Erreurs avec assurance : <carte : idée fausse, ou « aucune »>
- Carte d'application : réussie | partielle | non réussie | sautée
- Prochains rappels : <date vers J+2>, <date vers J+7> (chacune due séparément)
- Questions défectueuses : <ou « aucune »>
- Détail : historique/<fichier>.md | non conservé
```

### Synthèse

```
## AAAA-MM-JJ · Synthèse · <sujet> (<notions>)
- Conditions : <normales | sans rappel préalable>
- Forme : <tableau comparatif | enchaînement | plan de réponse à développement | vérification de syntheses/<fichier>.md>
- Faits de base manquants au départ : <notions, ou « aucun »>
- Construit sans aide (premier jet) : <notions ou liens>
- Ajouté avec les notes : <…>
- Encore flou : <notions, ou « rien »>
- Fichier : syntheses/<fichier>.md
- Vérification prévue : <une date, ou « sans objet » pour une vérification>
- Questions défectueuses : <ou « aucune »>
- Détail : historique/<fichier>.md | non conservé
```

### Quiz

```
## AAAA-MM-JJ · Quiz <diagnostic | variantes | espacé> · <Semaine N, séance k> (diagnostic) | <Semaines …> (variantes, espacé) [· rattrapage : Semaine N, séance k] [· mise à niveau] [(partiel)]
- Score : <x>/<y>
- Estimation de l'étudiant : <x>/<y> · Réel : <x>/<y>
- Maîtrisé : <notions> (réussites sûres seulement : juste, « sûr », conditions normales)
- Incomplet : <notions>
- Erroné : <notion : type d'erreur>
- Absent : <notions> (question posée, puis passée ou laissée sans réponse; une question jamais posée n'entre pas dans l'entrée)
- Erreurs de forme : <ou « aucune »>
- Conditions : <normales | rappel le jour même | notes consultées>
- Questions défectueuses : <ou « aucune »>
- Prochain quiz : <mode>, <une date>
- Détail : historique/<fichier>.md | non conservé
```

### Tutoriel

```
## AAAA-MM-JJ · Tutoriel · <notion> (Semaine N, séance k)
- Conditions : <normales | sans rappel préalable>
- Étapes réussies du premier coup : <…>
- Étapes reprises : <étape : idée fausse>
- Exemple final seul : réussi | partiel | non réussi | sauté
- À revoir : <…>
- Questions défectueuses : <ou « aucune »>
- Détail : historique/<fichier>.md | non conservé
```

### Plan de révision

```
## AAAA-MM-JJ · Plan de révision · Examen <n> (version <v>)
- Examen : <date>, semaines <…>, <pondération>
- Temps disponible : <heures par jour>
- Répartition : <partie : part du temps>; …
- Séances prévues (numérotées; l'examen blanc est une séance du plan) :
  1. <date> : <notions>, <activité>
  2. <date> : <notions>, <activité>
  …
  k. <date> : examen blanc
- Ce qui tombe faute de temps : <ou « rien »>
```

### Séance de révision

```
## AAAA-MM-JJ · Révision examen <n> · Séance <k> (plan v<v>)
- Notions travaillées : <…>
- Résultat : <x/y problèmes réussis>
- Conditions : <normales | notes consultées>
- Maîtrisé : <notions> (réussites sûres seulement : juste, « sûr », conditions normales)
- Erreurs : <notion : type d'erreur>
- Absent : <notions> (problème passé ou laissé sans réponse)
- Questions défectueuses : <ou « aucune »>
- Détail : historique/<fichier>.md | non conservé
```

### Examen blanc

```
## AAAA-MM-JJ · Examen blanc <n> · Séance <k> (plan v<v>)
- Note : <x> à <y>/100
- Estimation de l'étudiant : <x>/100 · Réel : <x> à <y>/100
- Conditions : <notes fermées et chronométré | écarts : …>
- Temps : <durée réelle> pour <durée prévue>
- Maîtrisé : <notions> (réussites sûres seulement)
- Erreurs : <notion : type d'erreur>
- Absent : <notions, ou « aucune »> (question laissée sans réponse)
- À reprendre avant l'examen : <au plus 5>
- Questions défectueuses : <ou « aucune »>
- Détail : historique/<fichier>.md | non conservé
```

### Copie corrigée

```
## AAAA-MM-JJ · Copie corrigée · <évaluation>
- Date de l'examen : AAAA-MM-JJ
- Fichier : copies-corrigees/<nom du fichier>
- Note : <x>/100 (examen blanc : <x> à <y>, s'il y en a eu un)
- Points perdus par type : contenu <n>, forme <n>, temps <n>, lecture <n>
- Notions touchées : <notion : réussie | points perdus>
- Écarts avec la carte : <…>
- Répartition de la préparation : <bien ciblée | sur-investi : … | sous-investi : …>
- Leçons pour le prochain examen : <au plus 3>
```

### Partie (Minerva-Jeux, regles-jeux.md)

Une partie notée sans analyse (jouée en personne, ou analyse remise à plus tard).

```
## AAAA-MM-JJ · Partie · <variante> contre <adversaire>
- Variante : <variante>
- Source : <plateforme, numéro de partie | en personne>
- Fichier : parties/<fichier> | aucun
- Format : <cadence, match en N points, etc.>
- Déroulement : <une ou deux lignes, sans jugement>
- Estimation de l'étudiant : <moments où il pense s'être trompé, ou « à faire »>
- Analyse : <à faire | non prévue>
```

### Analyse (Minerva-Jeux, regles-jeux.md)

```
## AAAA-MM-JJ · Analyse · <fichier>
- Variante : <variante>
- Moteur : <moteur, réglage>
- Indice d'erreur : <valeur et unité de la fiche; au backgammon : global, pions, videau>
- Estimation de l'étudiant : <ses moments, tels qu'il les a dits> · Réel : <n de ses moments parmi les erreurs retenues>
- Erreurs : <code : coup, ce qui s'est passé, coût>; <code : …>
- Notions ajoutées : <codes, ou « aucune »>
- Détail : historique/AAAA-MM-JJ-analyse-<fichier sans extension>.md
```

## Entrées

<!-- Les entrées s'ajoutent ici, la plus récente en bas. -->

## 2026-11-08 · Démarrage · Backgammon
- Structure créée : LISEZMOI.md, inbox/, parties/, historique/ (avec .preparation/ et entrees-importees/), journal-de-suivi.md
- Plan de cours : remplacé par le brief Minerva-Backgammon (notions de départ, cycle de travail, règles)
- Ressources à déposer : parties exportées de Backgammon Galaxy (.mat)
- Mise à niveau : sans objet

## 2026-11-08 · Partie · backgammon contre aquavision
- Variante : backgammon
- Source : Backgammon Galaxy, match 50384696
- Fichier : parties/2026-11-08-galaxy-50384696-aquavision.mat
- Format : match en 4 points, videau limité à 4
- Déroulement : une seule manche; double accepté au 5e coup, redouble à 4 au 11e coup; manche et match perdus
- Estimation de l'étudiant : « je jouais un peu n'importe comment », première partie
- Analyse : non prévue (première partie, bases d'abord)
- Notions en cause : non analysée

## 2026-11-08 · Partie · backgammon contre ww493535
- Variante : backgammon
- Source : Backgammon Galaxy, match 50409658
- Fichier : parties/2026-11-08-galaxy-50409658-ww493535.mat
- Format : match en 2 points, videau limité à 2
- Déroulement : double de l'adversaire au 13e coup, refusé; manche perdue 1 point; la suite du match n'est pas dans le fichier
- Estimation de l'étudiant : à faire (avait-il l'intention de refuser?)
- Analyse : à faire, décision de videau seulement
- Notions en cause : non analysée

## 2026-11-08 · Analyse · 2026-11-08-galaxy-50409658-ww493535.mat
- Variante : backgammon
- Moteur : GNU Backgammon 1.07, 2 plis (pions et videau)
- Indice d'erreur : global 109,6 mEMG · pions 173,4 · videau 0,1
- Estimation de l'étudiant : « je ne savais même ce qu'était le concept de doubler. Je pense avoir joué au tavla et ce concept ne semble pas exister. » · Réel : 0 de ses moments parmi les erreurs retenues (aucun moment nommé; le refus du double était correct; la partie est du backgammon, pas du tavla)
- Erreurs : frapper-ou-construire : 6e coup 53, bar/22 13/8 au lieu de bar/20* 13/10* (double frappe manquée), −1,220, et 3e coup 65, 24/13 au lieu de 7/1* 6/1, −0,296; construire-points : 2e coup 51, 13/8 7/6 défait la barre faite au coup précédent et laisse deux pions seuls (24/18 recommandé), −0,401; prime-et-ancre : 5e coup 62, 24/22 13/7 au lieu de 24/18 20/18 (ancre sur la barre adverse), −0,163
- Notions ajoutées : aucune
- Détail : historique/2026-11-08-analyse-2026-11-08-galaxy-50409658-ww493535.md

## 2026-11-08 · Approfondir · frapper-ou-construire
- Conditions : normales
- Approfondi : frapper-ou-construire
- Encore flou : rien
- Vérification : faite
- Questions défectueuses : aucune
- Détail : historique/2026-11-08-approfondir-frapper-ou-construire.md

## 2026-11-08 · Tutoriel · frapper-ou-construire (Semaine 2, séance 1)
- Conditions : normales
- Étapes réussies du premier coup : repérer les pions frappables; risque et temps de la frappe (après relance sur le pourquoi)
- Étapes reprises : coût de la frappe : confond chemin restant et chemin perdu (réussie au remplacement); comparer frapper et construire : bon choix, justification complétée (les deux coups avancent de 6)
- Exemple final seul : non réussi
- À revoir : renoncer à frapper quand la frappe fait peu reculer l'adversaire et expose un pion seul au fond de son jan; vérifier qu'un coup est jouable avec les dés (24/18 proposé avec 4-2)
- Questions défectueuses : aucune
- Détail : historique/2026-11-08-tutoriel-frapper-ou-construire.md
