# Installer NOVARIUM

## Windows 11 x64

Télécharger uniquement l’archive versionnée depuis les [Releases officielles](https://github.com/Light-x02/Novarium/releases). Son empreinte SHA-256 figure sur la page de version ; elle doit correspondre au fichier téléchargé.

Extraire complètement l’archive. Dans le dossier `NOVARIUM`, conserver ensemble `NOVARIUM.exe`, `LANCER_WEB.bat`, `_internal` et les autres ressources. Le programme utilise une distribution en dossier, pas un EXE isolé. Aucun Python ni Node.js n’est requis.

## Choisir son mode

**Fenêtre Windows** : ouvrir `NOVARIUM.exe`. Installer le Runtime Evergreen Microsoft Edge WebView2 s’il est signalé manquant, depuis [Microsoft](https://developer.microsoft.com/microsoft-edge/webview2/).

**Navigateur** : ouvrir `LANCER_WEB.bat`. Le serveur local utilise `http://127.0.0.1:8766/` et reste limité à cet ordinateur. Garder la console ouverte et utiliser **Ctrl+C** pour arrêter proprement le serveur. L’ouverture automatique du navigateur se règle dans les paramètres. Le mode web ne nécessite pas WebView2.

Fermer un mode avant de lancer l’autre. En cas de port occupé, fermer l’autre instance concernée ; NOVARIUM n’arrête pas un programme tiers pour libérer son port.

## Profils et données

Choisir ou créer un profil. Les données se trouvent par défaut sous `%LOCALAPPDATA%\NOVARIUM\`, séparées du dossier du programme. L’emplacement de la base et les sauvegardes se gèrent dans **Paramètres → Données et sauvegardes**. Ne supprimer aucun dossier de données lors d’une mise à jour.

Pour récupérer des métadonnées, configurer les services souhaités dans les paramètres. Les clés restent locales ; aucune clé de l’éditeur n’est distribuée. Certains services imposent une inscription, un quota ou un abonnement distinct.

## Mettre à jour

Dans **Paramètres → Mises à jour**, lancer une recherche ou conserver la recherche au démarrage. Le téléchargement est vérifié avant installation. Enregistrer les modifications et terminer les imports avant de confirmer **Fermer et installer**. L’ancien programme est conservé ; les données ne sont pas remplacées.

Tant que le dépôt de téléchargement est privé, son accès nécessite une autorisation GitHub configurée localement. Lorsque ce même dépôt sera public, aucun compte ni jeton GitHub ne sera nécessaire pour télécharger les versions publiques. Aucun jeton personnel n’est embarqué.

Une ancienne version du programme peut ne pas être compatible avec une base plus récente. Effectuer une sauvegarde et vérifier la compatibilité du schéma avant un retour en arrière.

## Dépannage

Si Windows ou un antivirus bloque un fichier, conserver le détail de l’alerte, la version et l’empreinte du fichier pour le signalement. Ne pas désactiver les protections pour contourner un avertissement inexpliqué. Le programme n’est pas annoncé comme signé tant qu’une signature de code vérifiable n’est pas fournie.

Les installateurs Windows pourront être ajoutés ultérieurement ; la version actuellement proposée est une archive à extraire.
