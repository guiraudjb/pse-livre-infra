# pse-livre-infra

Révision, chapitre par chapitre, du livre « Infrastructure informatique d'une grande organisation publique : exigences, architecture, résilience » (37 modules, lecture audio synchronisée avec les pages).

**Site autonome** : https://guiraudjb.github.io/pse-livre-infra/ (page `index.html` à la racine,
`catalogue.json` limité à ce dépôt). Ses modules apparaissent aussi dans l'application commune
https://guiraudjb.github.io/PSE25-27/.

`index.html`, `sw.js` et les icônes sont une copie de la page commune
(`PSE25-27/`) : les modifier là-bas puis lancer `scripts/sync-web.py`, jamais ici.

## Le livre

Ouvrage personnel rédigé avec l'aide de l'IA par une personne qui prépare une qualification informatique
ministérielle (pseudonyme Arducible, novembre 2026). Le ministère qui sert de fil rouge est fictif.

## Série

- **20** : Livre : infrastructure informatique publique. 20-00 préface et introduction, 20-01 à 20-35 les
  chapitres, 20-36 les annexes.

## Contenu de chaque module

Dans `batocera/pse-livre-infra/data/` :

- `fiche/`, `quizz/`, `flashcard/` : fiche de révision, QCM et flashcards (pipeline local, gemma4) ;
- `infographie/`, `podcast/`, `chanson/` (slam), `icone/` : médias du pipeline local ;
- `fiche_audio/` : **lecture du chapitre par Amélie** (livre audio, version standard) ;
- `source/` + `sources.json` : le chapitre en PDF, le livre complet et sa version rédigée (onglet SOURCES) ;
- `lecture/` : onglet **LECTURE**. Livre audio synchronisé avec les pages du PDF, en version standard ou
  en version rédigée (style administratif) : `index.json`, `<version>.json` (instants de changement de page,
  lignes horodatées), `pages_<version>/` (images des pages), `audio_bis/` (lecture de la version rédigée).

Le jeu Batocera est dans `batocera/pse-livre-infra/` (moteur commun, recopié par `scripts/sync-batocera.py`).
