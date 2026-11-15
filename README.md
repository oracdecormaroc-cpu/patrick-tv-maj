# Patrick TV · mises à jour

Ce dépôt sert uniquement à distribuer les nouvelles versions de Patrick TV.

- `version.json` : la dernière version (numéro, notes, lien de l'APK pour chaque box).
- `apk/` : les APK (`mibox` pour la Xiaomi TV Box, `googletv` pour les télés Google TV).

L'appli lit `https://raw.githubusercontent.com/oracdecormaroc-cpu/patrick-tv-maj/HEAD/version.json`
quelques secondes après le démarrage. Si `versionCode` est plus grand que celui installé, elle propose
« Installer ». On peut aussi lancer la vérification dans Réglages → Mises à jour.

Pour publier une version : déposer les deux APK dans `apk/`, puis mettre à jour `version.json`
(versionCode, versionName, notes, liens). Les APK doivent être signés avec la même clé.
