# Lionel 🦁

Jeu de mots quotidien : rejoins le mot **LION** en changeant une seule lettre à la fois.

## Règles
- Chaque jour, un nouveau mot de départ (à distance minimale de 4 de LION)
- Tape un mot de 4 lettres au clavier : il doit exister dans le dictionnaire et différer du mot précédent d'une seule lettre exactement
- Chaque mot validé s'ajoute à la chaîne, enchaîne jusqu'à LION
- Le score final compare ton nombre de coups au chemin optimal

## Jouer
- Ouvrir index.html dans un navigateur, ou
- Activer GitHub Pages : Settings → Pages → Deploy from a branch → main / root

## Tech
- HTML/CSS/JS vanilla, zéro dépendance — léger et rapide sur mobile
- Le mot du jour est déterministe (fonction de la date locale) : tout le monde a le même
- Progression du jour sauvegardée en localStorage, remise à zéro à minuit
- Clavier AZERTY à l'écran + support du clavier physique

## Dictionnaire
2657 mots français de 4 lettres (source : listesdemots.net), sans accents (style Scrabble).
Les mots de départ sont ceux à distance BFS >= 4 de LION (2442 éligibles).