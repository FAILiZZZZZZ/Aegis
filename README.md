# Aegis

Filtre de loot original pour **Path of Exile 2**, conçu pour le **Softcore Trade endgame**.

> Statut : en développement actif — version actuelle du filtre : **0.2.0**.

## Objectif

Aegis est un filtre **TradeStrict+** : il vise à réduire fortement le bruit visuel tout en conservant les objets utiles, recherchés ou incertains pour le commerce.

Ses priorités actuelles sont :

- économie et objets endgame ;
- builds caster / Spirit Walker ;
- équipements avec Energy Shield, y compris les bases hybrides ;
- sécurité : en cas de doute sur la valeur d'un objet, le filtre privilégie l'affichage plutôt que le masquage.

## Fonctionnement actuel

| Catégorie | Comportement |
| --- | --- |
| Monnaies | Paliers visuels S+ à C ; Transmutation, Augmentation et Regal de tier 1 masqués. |
| Gemmes brutes | Gemmes d'Aptitude et d'Esprit affichées à partir du niveau 17 ; niveau 20 mis en avant. |
| Runes | Runes premium mises en avant ; autres socketables conservés par sécurité. |
| Waystones | T15 et T16 affichées avec une priorité élevée. |
| Équipement rare | Affiché à partir de l'ilvl 82, ainsi que les rares possédant de l'Energy Shield. |
| Uniques | Bagues, amulettes et ceintures toujours visibles ; les autres uniques restent visibles tant que la liste manuelle de chase uniques est incomplète. |
| Contenu endgame | Tablettes, fragments, logbooks et reliques affichés. |
| Essais | Djinn Barya et Inscribed Ultimatum masqués. |
| Reste du butin | Masqué par la règle finale du filtre. |

## Niveaux visuels

| Niveau | Couleur | Usage |
| --- | --- | --- |
| S+ | Rouge / violet | Objets exceptionnels. |
| S | Vert | Objets de très haute valeur ou priorité. |
| A | Jaune | Objets endgame importants. |
| B | Bleu | Objets utiles ou de valeur intermédiaire. |
| C | Blanc | Objets conservés par prudence. |

Les niveaux **S+** et **S** déclenchent également un son.

## Installation

1. Télécharge [Aegis.filter](Aegis.filter).
2. Copie le fichier dans le dossier de filtres de Path of Exile 2 :

   ```text
   Documents\My Games\Path of Exile 2
   ```

3. Dans le jeu, ouvre les options puis l'onglet **UI**.
4. Sélectionne `Aegis.filter` dans la liste des filtres d'objets.

Après une mise à jour, remplace simplement l'ancien fichier par la nouvelle version puis recharge-le dans les options du jeu.

## Développement

Le projet est volontairement maintenu dans un seul fichier : [`Aegis.filter`](Aegis.filter). Cela permet de lire et d'ajuster les règles directement, sans générateur ni étape de compilation.

Les évolutions prévues sont notamment :

- liste manuelle des chase uniques ;
- affinage des niveaux économiques selon l'utilité durable ;
- règles plus précises pour les bases ES et hybrides ;
- ajustements après tests en jeu.

## Versions

Les commits enregistrent les évolutions du projet. Une **release GitHub** sera créée pour chaque version testée et prête à être utilisée, afin de pouvoir télécharger facilement une version stable d'Aegis.
