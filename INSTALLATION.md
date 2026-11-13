# Installer NOVARIUM 0.49.0

## Configuration Windows

- **Windows 11 x64** : système utilisé pour les tests de NOVARIUM.
- **Windows 10 22H2 x64** : compatibilité prévue d’après les composants utilisés, mais pas encore vérifiée par un test complet de NOVARIUM sous Windows 10.

Cette archive est destinée aux PC x64. La compatibilité Windows 32 bits et ARM64 n’est pas validée.

## Composants requis

- **Microsoft Edge WebView2 Runtime Evergreen** : déjà inclus dans Windows 11 et présent sur la plupart des PC Windows 10. S’il manque, télécharger le **Evergreen Bootstrapper** depuis [Microsoft](https://developer.microsoft.com/microsoft-edge/webview2/#download), l’exécuter, puis relancer NOVARIUM. Pour une installation hors ligne, choisir **Evergreen Standalone Installer — x64**. Le navigateur Edge seul ne remplace pas ce composant.
- **.NET Framework 4.8 ou ultérieur** : normalement présent dans Windows 10 22H2 et Windows 11. S’il est absent ou endommagé, utiliser le [Runtime .NET Framework 4.8 de Microsoft](https://dotnet.microsoft.com/en-us/download/dotnet-framework/net48), puis redémarrer Windows si l’installation le demande. Aucun pack de développement n’est nécessaire.

Ces composants sont pris en charge sous Windows 10 et Windows 11 selon la [documentation WebView2](https://learn.microsoft.com/en-us/microsoft-edge/webview2/) et la [documentation .NET Framework](https://learn.microsoft.com/en-us/dotnet/framework/install/versions-and-dependencies). Cela ne remplace pas une validation réelle de NOVARIUM sur chaque système.

## Télécharger et extraire

Télécharger **[NOVARIUM-v0.49.0.zip](https://github.com/Light-x02/Novarium/releases/download/v0.49.0/NOVARIUM-v0.49.0.zip)** depuis la release officielle. L’empreinte SHA-256 permet de vérifier le téléchargement.

Extraire complètement l’archive. Dans le dossier `NOVARIUM`, conserver ensemble `NOVARIUM.exe`, `_internal` et toutes les ressources fournies. Le programme utilise une distribution en dossier, pas un EXE isolé.

## Ouvrir NOVARIUM

Ouvrir **`NOVARIUM.exe`**. L’application s’affiche dans sa propre fenêtre Windows. Installer le Runtime Evergreen Microsoft Edge WebView2 s’il est signalé manquant, depuis [Microsoft](https://developer.microsoft.com/microsoft-edge/webview2/).

Ne pas supprimer les fichiers annexes du dossier du programme. Si une instance est déjà ouverte, l’enregistrer et la fermer normalement avant de relancer NOVARIUM.

## Profils et données

Au premier lancement, créez votre profil. Un guide de bienvenue vous accompagne pour configurer les sources de métadonnées ; vous pouvez passer cette étape et y revenir plus tard. Les données se trouvent par défaut sous `%LOCALAPPDATA%\NOVARIUM\`, séparées du dossier du programme. L’emplacement de la base et les sauvegardes se gèrent dans **Paramètres → Données et sauvegardes**. Ne supprimer aucun dossier de données lors d’une mise à jour.

Le crayon d’un profil permet de le modifier, de le dupliquer ou de le supprimer. La suppression demande une confirmation explicite et le nom exact du profil. Les sauvegardes et fichiers externes sont conservés.

Pour récupérer des métadonnées, configurez les services souhaités dans **Paramètres → Métadonnées et services**. Le bouton **Guide de bienvenue et clés API** permet de retrouver les instructions. Les clés restent locales ; aucune clé de l’éditeur n’est distribuée. Certains services imposent une inscription, un quota ou un abonnement distinct.

## Mettre à jour

Dans **Paramètres → Mises à jour**, lancer une recherche ou conserver la recherche au démarrage. Le téléchargement est vérifié avant installation. Enregistrer les modifications et terminer les imports avant de confirmer **Fermer et installer**. L’ancien programme est conservé ; les données ne sont pas remplacées.

Le dépôt de téléchargement est public : aucun compte ni jeton GitHub n’est nécessaire pour télécharger les versions et utiliser la recherche de mises à jour.

Une ancienne version du programme peut ne pas être compatible avec une base plus récente. Effectuer une sauvegarde et vérifier la compatibilité du schéma avant un retour en arrière.

## Dépannage

Si Windows ou un antivirus bloque un fichier, conserver le détail de l’alerte, la version et l’empreinte du fichier pour le signalement. Ne pas désactiver les protections pour contourner un avertissement inexpliqué. Le programme n’est pas annoncé comme signé tant qu’une signature de code vérifiable n’est pas fournie.

La version proposée est une archive à extraire.

Pour une question d’installation ou d’utilisation, consultez [Questions et aide](https://github.com/Light-x02/Novarium/discussions/categories/questions-et-aide). Pour proposer une amélioration, utilisez [Idées et suggestions](https://github.com/Light-x02/Novarium/discussions/categories/id%C3%A9es-et-suggestions). Les [Issues](https://github.com/Light-x02/Novarium/issues) permettent de signaler les bugs. Ne partagez aucun identifiant secret ni fichier personnel.

## Sauvegarder et transférer

Dans **Paramètres → Données et sauvegardes**, vous pouvez planifier des sauvegardes, restaurer une copie et exporter un profil complet ou des collections.

- **Sauvegardes automatiques** : les liens vers les vidéos et leurs associations aux films et épisodes sont conservés.
- **Export d’un profil complet** : l’option **Inclure les liens des vidéos locales** est cochée par défaut.
- **Export de collections** : cette option est décochée par défaut, pour faciliter le partage sans vos chemins de fichiers.
- **Aucun fichier vidéo n’est inclus** : les liens fonctionnent si les vidéos sont accessibles au même emplacement. Sur un autre PC, vous pouvez associer vos propres fichiers depuis **Modifier la fiche**.

Un export préparé reste accessible dans **Importer / exporter** après un changement de page. Vous pouvez le télécharger ou l’annuler.

## Versions et compatibilité des données

La mise à jour de la 0.48.0 vers la 0.49.0 conserve les profils, les réglages, les bibliothèques et les associations aux vidéos locales. Conservez vos sauvegardes avant toute mise à jour.

Les anciennes éditions de développement, antérieures au socle public 0.46.0, utilisent un autre format. Elles ne doivent pas ouvrir une bibliothèque récente et leurs anciens profils ne sont pas convertis. Si un nouveau départ est proposé pour ces éditions, les anciens fichiers sont conservés séparément.

L’analyse de la qualité vidéo est intégrée : aucun outil supplémentaire n’est à installer. Conservez tous les fichiers fournis avec le programme.

## Vérifier le téléchargement

SHA-256 de **`NOVARIUM-v0.49.0.zip`** :

```text
4d01c15fa9d8eeec1479d6c0c6787fd6695ef2b2ccc88968f237777ba6968d08
```
