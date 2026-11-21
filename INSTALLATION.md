# Installer NOVARIUM 0.51.1

## Configuration Windows

- **Windows 11 x64** : système utilisé pour les tests de NOVARIUM.
- **Windows 10 22H2 x64** : compatibilité prévue d’après les composants utilisés, mais pas encore vérifiée par un test complet de NOVARIUM sous Windows 10.

Cette archive est destinée aux PC x64. La compatibilité Windows 32 bits et ARM64 n’est pas validée.

## Composants requis

- **Microsoft Edge WebView2 Runtime Evergreen** : déjà inclus dans Windows 11 et présent sur la plupart des PC Windows 10. S’il manque, télécharger le **Evergreen Bootstrapper** depuis [Microsoft](https://developer.microsoft.com/microsoft-edge/webview2/#download), l’exécuter, puis relancer NOVARIUM. Pour une installation hors ligne, choisir **Evergreen Standalone Installer — x64**. Le navigateur Edge seul ne remplace pas ce composant.
- **.NET Framework 4.8 ou ultérieur** : normalement présent dans Windows 10 22H2 et Windows 11. S’il est absent ou endommagé, utiliser le [Runtime .NET Framework 4.8 de Microsoft](https://dotnet.microsoft.com/en-us/download/dotnet-framework/net48), puis redémarrer Windows si l’installation le demande. Aucun pack de développement n’est nécessaire.

Ces composants sont pris en charge sous Windows 10 et Windows 11 selon la [documentation WebView2](https://learn.microsoft.com/en-us/microsoft-edge/webview2/) et la [documentation .NET Framework](https://learn.microsoft.com/en-us/dotnet/framework/install/versions-and-dependencies). Cela ne remplace pas une validation réelle de NOVARIUM sur chaque système.

## Télécharger et extraire

Télécharger **[NOVARIUM-v0.51.1.zip](https://github.com/Light-x02/Novarium/releases/download/v0.51.1/NOVARIUM-v0.51.1.zip)** depuis la publication officielle. Le ZIP contient tout ce qui est nécessaire à l’installation de NOVARIUM. L’empreinte SHA-256 figure en bas de ce guide.

Extraire complètement l’archive. Dans le dossier `NOVARIUM`, conserver ensemble `NOVARIUM.exe`, `_internal` et toutes les ressources fournies. Le programme utilise une distribution en dossier, pas un EXE isolé.

## Ouvrir NOVARIUM

Ouvrir **`NOVARIUM.exe`**. L’application s’affiche dans sa propre fenêtre Windows. Installer le Runtime Evergreen Microsoft Edge WebView2 s’il est signalé manquant, depuis [Microsoft](https://developer.microsoft.com/microsoft-edge/webview2/).

Ne pas supprimer les fichiers annexes du dossier du programme. Si une instance est déjà ouverte, l’enregistrer et la fermer normalement avant de relancer NOVARIUM.

## Profils et données

Au premier lancement, créez votre profil. Un guide de bienvenue vous accompagne pour configurer les sources de métadonnées ; vous pouvez passer cette étape et y revenir plus tard. Les données se trouvent par défaut sous `%LOCALAPPDATA%\NOVARIUM\`, séparées du dossier du programme. L’emplacement de la base et les sauvegardes se gèrent dans **Paramètres → Données et sauvegardes**. Ne supprimer aucun dossier de données lors d’une mise à jour.

Le crayon d’un profil permet de le modifier, de le dupliquer ou de le supprimer. La suppression demande une confirmation explicite et le nom exact du profil. Les sauvegardes et fichiers externes sont conservés. Si le dossier actif est inaccessible, **Retirer du sélecteur** permet de retirer le profil de la liste en conservant ses fichiers.

Pour récupérer des métadonnées, configurez les services souhaités dans **Paramètres → Métadonnées et services**. Le bouton **Guide de bienvenue et clés API** permet de retrouver les instructions. Les clés restent locales ; aucune clé de l’éditeur n’est distribuée. Certains services imposent une inscription, un quota ou un abonnement distinct.

## Mettre à jour

Dans **Paramètres → Mises à jour**, lancer une recherche ou conserver la recherche au démarrage. Sélectionner **Télécharger la mise à jour**, puis **Fermer et installer** après avoir enregistré vos modifications et terminé vos imports. NOVARIUM conserve une copie de l’ancien programme et redémarre automatiquement. Un résumé des nouveautés s’affiche au premier lancement après la mise à jour. Pour les mises à jour lancées depuis la 0.51.1 ou une version ultérieure, NOVARIUM remet en place l’installation précédente si le nouveau programme se ferme avant de confirmer son ouverture.

Pour passer de la **0.49.0 à la 0.50.0**, la 0.49.0 télécharge le ZIP et vérifie son empreinte SHA-256. À partir de la **0.50.0**, l’application récupère également le fichier `.sig.json` et vérifie la signature Ed25519 avec sa clé publique intégrée. Le parcours automatique se fait entièrement depuis l’application.

Le dépôt de téléchargement est public : aucun compte ni jeton GitHub n’est nécessaire pour télécharger les versions et utiliser la recherche de mises à jour.

Une ancienne version du programme peut ne pas être compatible avec une base plus récente. Effectuer une sauvegarde et vérifier la compatibilité du schéma avant un retour en arrière.

## Dépannage

Si Windows ou un antivirus bloque un fichier, conserver le détail de l’alerte, la version et l’empreinte du fichier pour le signalement. La signature Ed25519 est vérifiée par NOVARIUM et porte sur l’archive de mise à jour. La vérification de l’exécutable par Windows relève de la signature de code Authenticode.

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

La mise à jour de la 0.51.0 vers la 0.51.1 a été testée avec les exécutables Windows et un profil fictif. Après redémarrage, la collection, les favoris, les notes, les préférences et la sauvegarde déjà présente ont été retrouvés. La transition de la 0.49.0 vers la 0.50.0 a aussi été vérifiée. Conservez vos sauvegardes avant toute mise à jour.

Les anciennes éditions de développement, antérieures au socle public 0.46.0, utilisent un autre format. Elles ne doivent pas ouvrir une bibliothèque récente et leurs anciens profils ne sont pas convertis. Si un nouveau départ est proposé pour ces éditions, les anciens fichiers sont conservés séparément.

L’analyse de la qualité vidéo est intégrée : aucun outil supplémentaire n’est à installer. Conservez tous les fichiers fournis avec le programme.

## Vérifier le téléchargement

SHA-256 de **`NOVARIUM-v0.51.1.zip`**

```text
e9e4e2a023f78fbe6774a3f52f6f4658d310ecdd387311bb4253b5fb2dc82fe1
```

Le fichier [`.sig.json`](https://github.com/Light-x02/Novarium/releases/download/v0.51.1/NOVARIUM-v0.51.1.zip.sig.json) contient la signature de cette archive. Lors d’une mise à jour depuis la 0.50.0 ou une version ultérieure, l’application le télécharge et le vérifie automatiquement. Pour installer le programme manuellement, le ZIP suffit. Le fichier de signature est disponible si vous souhaitez vérifier vous-même l’archive avec une copie de confiance de la clé publique.
