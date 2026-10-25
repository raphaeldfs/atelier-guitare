# Atelier guitare — installation

Ce dossier contient ton appli complète. Elle se met en ligne gratuitement avec GitHub Pages, puis s'installe sur ton téléphone et ton ordinateur comme une vraie appli, avec son icône. Compte environ 15 minutes la première fois, sur un ordinateur.

## Contenu du dossier

| Fichier | Rôle |
| --- | --- |
| `index.html` | L'appli elle-même |
| `manifest.webmanifest` | Nom, icône et couleurs pour l'installation |
| `sw.js` | Permet à l'appli de fonctionner hors connexion |
| `icons/` | Les icônes (médiator) |
| `mon-repertoire.json` | Ton répertoire actuel, à importer une fois (étape 4) |
| `LISEZ-MOI.md` | Ce guide |

## 1. Créer un compte GitHub

1. Va sur https://github.com et clique sur **Sign up**.
2. Choisis un nom d'utilisateur : il apparaîtra dans l'adresse de ton appli (`https://ton-nom.github.io/atelier-guitare/`).
3. Valide ton adresse mail.

## 2. Mettre l'appli en ligne

1. Une fois connecté, clique sur **+** en haut à droite, puis **New repository**.
2. Nom du dépôt : `atelier-guitare`. Coche **Public** (obligatoire pour GitHub Pages gratuit). Clique sur **Create repository**.
3. Sur la page du dépôt vide, clique sur le lien **uploading an existing file**.
4. Dézippe le dossier `atelier-guitare`, puis glisse **tout son contenu** dans la zone (les fichiers et le dossier `icons`, pas le dossier parent lui-même). Vérifie que `index.html` est bien à la racine dans la liste.
5. En bas, clique sur **Commit changes**.
6. Va dans **Settings** (onglet du dépôt), puis **Pages** dans le menu de gauche.
7. Sous **Build and deployment**, choisis **Source : Deploy from a branch**, **Branch : main**, dossier **/ (root)**, puis **Save**.
8. Attends 1 à 2 minutes et recharge la page : l'adresse de ton appli s'affiche en haut (`https://ton-nom.github.io/atelier-guitare/`).

Le dépôt est public : n'importe qui peut voir le code de l'appli, mais **pas tes données**, qui restent uniquement sur tes appareils.

## 3. Installer l'appli

**iPhone / iPad** : ouvre l'adresse dans **Safari** (pas Chrome), touche le bouton **Partager**, puis **Sur l'écran d'accueil**. L'icône du médiator apparaît ; l'appli s'ouvre en plein écran, sans barre d'adresse.

**Android** : ouvre l'adresse dans **Chrome**, menu **⋮**, puis **Installer l'application** (ou **Ajouter à l'écran d'accueil**).

**Ordinateur (Chrome ou Edge)** : ouvre l'adresse, puis clique sur l'icône d'installation à droite de la barre d'adresse (un écran avec une flèche). L'appli s'ouvre dans sa propre fenêtre.

Après la première ouverture, l'appli fonctionne même hors connexion (sauf les vidéos et Songsterr, qui demandent Internet).

## 4. Récupérer ton répertoire actuel

Sur chaque appareil, une seule fois :

1. Ouvre l'appli, menu **Mon répertoire**.
2. Dans **Passer d'un appareil à l'autre**, touche **Importer un fichier** et choisis `mon-repertoire.json`.
3. Confirme avec **Remplacer**.

## 5. Synchroniser entre tes appareils

Tes données (répertoire, records, progression du cours) sont enregistrées sur chaque appareil séparément. Pour passer de l'un à l'autre :

1. Sur l'appareil à jour : **Mon répertoire → Exporter mes données**. Un fichier `atelier-guitare-AAAA-MM-JJ.json` est téléchargé.
2. Envoie-le sur l'autre appareil (AirDrop, mail, iCloud Drive, Google Drive…).
3. Sur l'autre appareil : **Importer un fichier**, puis **Remplacer**.

L'import **remplace** les données de l'appareil : exporte toujours depuis celui que tu as modifié en dernier.

## Vidéos et tablatures

- Le bouton **▶ Vidéo** d'un morceau ouvre la vidéo YouTube directement dans l'appli, au moment indiqué dans le lien (`?t=95`).
- Le bouton **Tab Songsterr** essaie d'afficher la recherche Songsterr dans l'appli. Si la fenêtre reste vide ou affiche une erreur, c'est que Songsterr refuse d'être affiché dans un autre site : utilise alors le lien « ouvre-le dans un onglet ».
- Ultimate Guitar s'ouvre toujours dans un onglet séparé.

## Mettre à jour l'appli plus tard

Quand je te prépare une nouvelle version : dans ton dépôt GitHub, **Add file → Upload files**, glisse les nouveaux fichiers (ils remplacent les anciens), puis **Commit changes**. L'appli se met à jour à sa prochaine ouverture avec Internet. Tes données ne sont pas touchées.
