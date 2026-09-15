# Lionel 🦁

Jeu de mots quotidien : rejoins le mot **LION** en changeant une seule lettre à la fois.

## Règles
- Chaque jour, un nouveau mot de départ commun, à distance minimale de 4 de LION
- Tape un mot de 4 lettres au clavier : il doit exister dans le dictionnaire et différer du mot précédent d'une seule lettre exactement
- Chaque mot validé s'ajoute à la chaîne, enchaîne jusqu'à LION
- Les lettres à la bonne place (celles de LION) s'affichent en doré
- Le score final compare ton nombre de coups au chemin optimal
- À la victoire, le chemin optimal (plus court chemin vers LION) est révélé
- Une popup d'introduction avec le lore de Lionel apparaît au premier lancement

## Jouer
- Ouvrir index.html dans un navigateur, ou
- Activer GitHub Pages : Settings → Pages → Deploy from a branch → main / root

## Tech
- HTML/CSS/JS vanilla, zéro dépendance — léger et rapide sur mobile
- Le mot du jour est déterministe (fonction de la date locale) : tout le monde a le même
- Progression du jour sauvegardée en localStorage, remise à zéro à minuit
- Clavier AZERTY à l'écran + support du clavier physique

## Dictionnaire
- Validation des propositions : 2657 mots français de 4 lettres (listesdemots.net), sans accents (style Scrabble), verbes conjugués inclus
- Mots de départ : restreints aux mots courants du top 10 000 de fréquence (Wiktionary), filtrés par distance BFS >= 4 à LION (~300 candidats)
