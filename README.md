# C TOUT VU — Compteur régie

Application web légère pour le comptage des points de C TOUT VU en régie.

Un seul fichier HTML autonome, aucune dépendance, fonctionne dans tous les navigateurs modernes.

## Multi-appareil

La même URL fonctionne sur ordinateur, tablette et téléphone. L'application détecte automatiquement la taille de l'écran et adapte la mise en page :

- **Ordinateur / grand écran** : layout large, 3 duos côte à côte, navigation en haut
- **Tablette** : layout intermédiaire, cartes adaptées
- **Téléphone** : layout portrait, duos empilés verticalement, boutons XXL, navigation en bas de l'écran pour un accès rapide au pouce

Pour un usage régie confortable sur téléphone, tu peux "ajouter à l'écran d'accueil" depuis Safari ou Chrome pour lancer l'app en plein écran comme une vraie app native.

## Logo

Pour afficher le vrai logo de l'émission, déposer un fichier `logo.png` à la racine du dossier (au même niveau que `index.html`). L'app le charge automatiquement s'il est présent, et retombe sur un logo stylisé en CSS s'il ne trouve rien.

## Utilisation locale

Double-cliquer sur `index.html` pour ouvrir l'application dans le navigateur par défaut.

Les données sont sauvegardées automatiquement dans le navigateur (localStorage).

## Publier sur GitHub Pages

1. Créer un nouveau repo sur GitHub, par exemple `ctoutvu-compteur`.
2. Cloner ou uploader les fichiers `index.html` et `README.md` à la racine.
3. Dans le repo GitHub, ouvrir Settings > Pages.
4. Dans "Source", sélectionner la branche `main` et le dossier `/ (root)`, puis Save.
5. Attendre 1 à 2 minutes. L'app sera accessible à l'adresse `https://<ton-username>.github.io/ctoutvu-compteur/`.

## Fonctionnalités

- Configuration des 3 duos (noms des candidats, caméras, statut Champion en titre)
- Cagnotte reportée saisie manuellement
- Manche 1 (Le carré) : 25 €/bonne réponse, bonus 50 € si tableau complet
- Manche 2 (La roulette) : 25 €/bonne réponse, bonus 50 € par série de 4 consécutives
- Photo Finish après Manche 2 (25 €)
- Manche 3 (La battle) : 50 €/bonne réponse, bonus 100 € si tableau complet, 50 €/vol, bonus 100 € si tableau entier volé
- Photo Finish après Manche 3 (50 €)
- Manche 4 (Finale) : décompte des 12 images avec palier automatique
  - Moins de 8 : 0 €
  - 8 à 9 : cagnotte + cagnotte reportée
  - 10 à 11 : cagnotte + cagnotte reportée + 500 €
  - 12 : jackpot forfaitaire de 2 500 €
- Historique persistant des émissions jouées avec cumul des gains par champion
- Export JSON d'une émission

## Raccourcis clavier

À venir dans une prochaine version.
