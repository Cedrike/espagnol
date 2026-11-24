# ¡A repasar! · Révisions d'espagnol (LLCER, bac 2027)

Un site léger, interactif et ludique pour réviser l'espagnol en vue du baccalauréat 2027 (spécialité LLCER, terminale). Tout tient dans un seul fichier, `espanol-llc.html`, sans connexion ni compte.

## Utiliser le site

- **En ligne** : ouvre `https://cedrike.github.io/espagnol/espanol-llc.html` dans ton navigateur.
- **Sur iPad ou téléphone** : ouvre le lien dans Safari, puis **Partager → Sur l'écran d'accueil** pour le lancer comme une application.
- **Hors ligne** : télécharge `espanol-llc.html` et ouvre-le dans un navigateur.

## Ce que contient le site

### Conjugaison
- 10 temps et modes : présent, indefinido, imperfecto, perfecto, pluscuamperfecto, futur, conditionnel, subjonctif présent, subjonctif imparfait, impératif affirmatif.
- 85 verbes : réguliers, irréguliers et pronominaux, avec filtre par catégorie.
- Deux formats de questions : phrases à trous en contexte (le temps est à déduire) ou formes isolées.

### Vocabulaire et connecteurs
- Connecteurs logiques, expressions pour donner son avis et nuancer, lexique pour analyser un document, société et culture.
- Un thème par thématique du programme de terminale LLCER :
  1. Représentations culturelles : entre imaginaires et réalités
  2. Dominations et insoumissions
  3. L'Espagne et l'Amérique latine dans le monde
- Exercices dans les deux sens (français → espagnol et espagnol → français).

### Fiches leçons
- 14 fiches de conjugaison : emploi, terminaisons, irréguliers, exemples et pièges.
- Une fiche de référence par thème de vocabulaire.
- Un bouton « S'entraîner sur cette fiche » ouvre les exercices correspondants.

### Types d'exercices
QCM, saisie libre (avec boutons d'accents), cartes à retourner, défi chronométré de 60 secondes.

### Jeu
XP et niveaux, 5 vies, combos, série de jours, 10 badges, classement de tes meilleurs scores et taux de réussite par thème.

## Ta progression

Elle est enregistrée dans le navigateur de l'appareil (`localStorage`). Elle ne se synchronise pas entre appareils et elle est perdue si tu vides les données du navigateur. Elle est aussi liée à l'adresse du site : si l'adresse change, la progression repart de zéro.

## Ajouter une thématique

Chaque thème de révision est un module de la liste `MODS` dans `espanol-llc.html`. Un module décrit :

- ses filtres (thèmes, sens, format…),
- une fonction qui génère les questions,
- éventuellement une liste de fiches (`lessons`).

Les types d'exercices, l'XP, les vies, les badges, le profil et les fiches fonctionnent ensuite automatiquement. Un commentaire dans le code détaille le format attendu.

## Limites connues

- Les formes verbales sont générées par des règles et des exceptions. Si une forme te paraît fausse, signale-la pour qu'elle soit corrigée.
- Le vocabulaire des thématiques est général : il n'est pas encore calé sur les œuvres étudiées en classe.
- L'impératif n'existe que pour les verbes non pronominaux, et seulement à l'affirmatif.
