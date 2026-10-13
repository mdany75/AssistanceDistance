# AssistanceDistance

Site d'assistance à distance : l'usager télécharge AnyDesk, l'ouvre et donne son numéro
de poste au technicien (par téléphone), qui se connecte ensuite.

Site statique (aucun serveur), hébergé sur GitHub Pages :
https://911.groupecouture.ca/ (redirigé depuis https://mdany75.github.io/AssistanceDistance/)

## Utilisation

1. Donner l'adresse du site à l'usager.
2. L'usager télécharge et ouvre `AnyDesk.exe` (sans installation), puis lit son numéro.
3. Le technicien saisit ce numéro dans AnyDesk ; l'usager clique « Accepter ».

## Configuration (`config.js`)

| Clé | Rôle |
|-----|------|
| `titre` | Titre affiché en haut |
| `anydeskUrl` | Lien de téléchargement d'AnyDesk |
