# Backgammon · Minerva-Jeux

Dossier d'apprentissage du backgammon (et du tavla) de Philippe, suivi avec la méthode Minerva. Le brief du projet : https://claude.ai/artifact/KQGbQaBxBtJZMFwAdvE7pz

## Ce qui va où

- `inbox/` : dépose tout ici, en particulier les parties exportées de Backgammon Galaxy (`.mat`). Claude les range.
- `parties/` : les parties rangées, nommées `AAAA-MM-JJ-galaxy-<match>-<adversaire>.mat`.
- `historique/` : le détail de chaque activité (questions, réponses exactes, verdicts), écrit par les skills.
- `journal-de-suivi.md` : la mémoire du système. La liste des notions, et une entrée par activité ou par partie. On n'y fait que des ajouts.

## Comment travailler

- **Jouer** : sur Backgammon Galaxy, puis exporter la partie dans `inbox/`. Une partie de tavla avec ta copine n'a pas de fichier : raconte-la si un point de règle t'a surpris.
- **Étudier** : `etudier-notion`, suivi ou non d'une notion. Les coups d'ouverture se travaillent en mode Mémoriser.
- **Vérifier** : `faire-quiz`, deux ou trois jours plus tard.
- **Analyser une partie** : `jeu-analyser-partie`. GNU Backgammon mesure chaque décision; avant de voir l'analyse, tu dis d'abord où tu penses t'être trompé.
- **Faire le point** : `jeu-faire-le-point` (pas `faire-le-point`, qui cacherait les notions faute de dates de séances).

## Règles propres au backgammon

- Le moteur dit ce qui est vrai : aucune position, aucun meilleur coup, aucune probabilité ne vient de la mémoire de Claude.
- Le résultat d'une partie ne prouve rien : les dés comptent. Seules les décisions sont commentées.

## Synchronisation

Ce dossier est le dépôt privé GitHub `deltarhophi/backgammon`. Avant de travailler sur l'ordinateur, fais `git pull`; après, `git commit` puis `git push`. Claude fait de même quand il travaille depuis le mobile.
