# Installer NOVARIUM

## Configuration Windows

- **Windows 11 x64** : système utilisé pour les tests de NOVARIUM.
- **Windows 10 22H2 x64** : compatibilité prévue d’après les composants utilisés, mais pas encore vérifiée par un test complet de NOVARIUM sous Windows 10.

Cette archive est destinée aux PC x64. La compatibilité Windows 32 bits et ARM64 n’est pas validée.

## Composants requis

- **Microsoft Edge WebView2 Runtime Evergreen** : déjà inclus dans Windows 11 et présent sur la plupart des PC Windows 10. S’il manque, télécharger le **Evergreen Bootstrapper** depuis [Microsoft](https://developer.microsoft.com/microsoft-edge/webview2/#download), l’exécuter, puis relancer NOVARIUM. Pour une installation hors ligne, choisir **Evergreen Standalone Installer — x64**. Le navigateur Edge seul ne remplace pas ce composant.
- **.NET Framework 4.8 ou ultérieur** : normalement présent dans Windows 10 22H2 et Windows 11. S’il est absent ou endommagé, utiliser le [Runtime .NET Framework 4.8 de Microsoft](https://dotnet.microsoft.com/en-us/download/dotnet-framework/net48), puis redémarrer Windows si l’installation le demande. Aucun pack de développement n’est nécessaire.

Ces composants sont pris en charge sous Windows 10 et Windows 11 selon la [documentation WebView2](https://learn.microsoft.com/en-us/microsoft-edge/webview2/) et la [documentation .NET Framework](https://learn.microsoft.com/en-us/dotnet/framework/install/versions-and-dependencies). Cela ne remplace pas une validation réelle de NOVARIUM sur chaque système.

## Télécharger et extraire

Télécharger uniquement l’archive versionnée depuis les [Releases officielles](https://github.com/Light-x02/Novarium/releases). L’empreinte SHA-256 indiquée par GitHub pour le fichier joint permet de vérifier le téléchargement.

Extraire complètement l’archive. Dans le dossier `NOVARIUM`, conserver ensemble `NOVARIUM.exe`, `_internal` et toutes les ressources fournies. Le programme utilise une distribution en dossier, pas un EXE isolé.

## Ouvrir NOVARIUM

Ouvrir **`NOVARIUM.exe`**. L’application s’affiche dans sa propre fenêtre Windows. Installer le Runtime Evergreen Microsoft Edge WebView2 s’il est signalé manquant, depuis [Microsoft](https://developer.microsoft.com/microsoft-edge/webview2/).

Ne pas supprimer les fichiers annexes du dossier du programme. Si une instance est déjà ouverte, l’enregistrer et la fermer normalement avant de relancer NOVARIUM.

## Profils et données

Choisir ou créer un profil. Les données se trouvent par défaut sous `%LOCALAPPDATA%\NOVARIUM\`, séparées du dossier du programme. L’emplacement de la base et les sauvegardes se gèrent dans **Paramètres → Données et sauvegardes**. Ne supprimer aucun dossier de données lors d’une mise à jour.

Le crayon d’un profil permet de modifier son identité ou de le dupliquer. La copie est indépendante. Pour les profils secondaires, **Supprimer le profil** exige la saisie du nom exact et retire définitivement les données actives dont l’appartenance est vérifiée. Le profil principal ne peut pas être supprimé. Les sauvegardes conservées et fichiers externes ne sont pas supprimés ; les réinitialisations restent des opérations distinctes.

Pour récupérer des métadonnées, configurer les services souhaités dans les paramètres. Les clés restent locales ; aucune clé de l’éditeur n’est distribuée. Certains services imposent une inscription, un quota ou un abonnement distinct.

## Mettre à jour

Dans **Paramètres → Mises à jour**, lancer une recherche ou conserver la recherche au démarrage. Le téléchargement est vérifié avant installation. Enregistrer les modifications et terminer les imports avant de confirmer **Fermer et installer**. L’ancien programme est conservé ; les données ne sont pas remplacées.

Le dépôt de téléchargement est public : aucun compte ni jeton GitHub n’est nécessaire pour télécharger les versions et utiliser la recherche de mises à jour.

Une ancienne version du programme peut ne pas être compatible avec une base plus récente. Effectuer une sauvegarde et vérifier la compatibilité du schéma avant un retour en arrière.

## Dépannage

Si Windows ou un antivirus bloque un fichier, conserver le détail de l’alerte, la version et l’empreinte du fichier pour le signalement. Ne pas désactiver les protections pour contourner un avertissement inexpliqué. Le programme n’est pas annoncé comme signé tant qu’une signature de code vérifiable n’est pas fournie.

Les installateurs Windows pourront être ajoutés ultérieurement ; la version actuellement proposée est une archive à extraire.

## Nouveau socle de données en 0.46.0

La 0.46.0 utilise un nouveau format de données, de sauvegardes et d’archives. Les anciens profils et exports ne sont pas convertis ni importables dans ce socle. Lorsqu’un ancien stockage est détecté, le programme demande confirmation avant de créer un espace vierge ; les anciens fichiers restent conservés. Gardez l’ancienne installation et ses sauvegardes pour consulter vos anciennes données. Une ancienne version ne doit pas ouvrir une base plus récente.

FFprobe est fourni : aucune installation de sonde vidéo n’est nécessaire. Conservez ses DLL et les sources et licences tierces jointes au dossier `_internal`.

SHA-256 de `NOVARIUM-v0.46.0.zip` :

```text
e3109cd8823f8ef1e4973c539e174222c6269bb8d9bfd509c289e7cfa694520d
```
