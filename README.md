# AssistanceDistance

Site d'assistance à distance : l'usager télécharge AnyDesk, entre son numéro de poste,
son nom et son téléphone, et le technicien reçoit une alerte dans Teams.

Site statique (aucun serveur), prévu pour GitHub Pages.

## Utilisation

1. Donner à l'usager l'adresse du site et le code d'accès (par téléphone).
2. L'usager suit les 3 étapes.
3. L'alerte arrive dans Teams avec le nom, le téléphone et le numéro AnyDesk.

## Configuration (`config.js`)

| Clé | Rôle |
|-----|------|
| `titre` | Titre affiché en haut |
| `codeAcces` | Code demandé avant d'afficher le formulaire |
| `webhookUrl` | URL du webhook Teams (voir ci-dessous) |
| `anydeskUrl` | Lien de téléchargement d'AnyDesk |

## Créer le webhook Teams

1. Dans Teams : conversation (ou canal) cible → `…` → **Workflows**.
2. Modèle **« Publier dans un canal quand une demande de webhook est reçue »**
   (ou « Post to a chat when a webhook request is received »).
3. Copier l'URL générée dans `webhookUrl` de `config.js`.

## Limites de sécurité

Le code d'accès et l'URL du webhook sont lisibles dans le code source du site.
Ce site convient pour un test ; en production, mettre une validation côté serveur.
