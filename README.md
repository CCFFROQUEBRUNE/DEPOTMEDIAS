# DEPOTMEDIAS — CCFF RSA

Plateforme de dépôt de médias (photos/vidéos) pour bénévoles, sans compte Google requis.

## Fichiers

| Fichier | Rôle |
|---|---|
| `depot.html` | Page bénévole (smartphone) |
| `admin.html` | Console administration |
| `Code.gs` | Apps Script (backend Google) |

## Utilisation

- Bénévole : `https://CCFFRoquebrune.github.io/DEPOTMEDIAS/depot.html?event=AGAD2026`
- Admin : `https://CCFFRoquebrune.github.io/DEPOTMEDIAS/admin.html`

## Ajouter un événement

Dans `Code.gs`, ajouter une entrée dans `EVENTS_CONFIG` :

```js
"NOM_EVENT": {
  folderId:       "ID_DOSSIER_DRIVE",
  photosFolderId: "ID_SOUS_DOSSIER_PHOTOS",
  videosFolderId: "ID_SOUS_DOSSIER_VIDEOS",
  code:           "1234",
  active:         true,
  quotaMo:        30,
  maxPhotoMo:     30,
  maxVideoMo:     100,
  label:          "Nom affiché"
}
```
