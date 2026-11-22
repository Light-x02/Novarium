# Vos données et votre confidentialité

NOVARIUM est une application locale. Aucun compte NOVARIUM distant n’est nécessaire. Collections, profils, notes, suivis, préférences et sauvegardes sont enregistrés sur votre ordinateur. Le programme n’intègre pas de service d’analyse d’usage NOVARIUM ni d’envoi automatique de vos collections à l’éditeur.

## Connexions externes

- Les recherches et imports de métadonnées transmettent les titres, identifiants ou critères nécessaires aux fournisseurs sélectionnés, dont TMDB, OMDb, Steam, IGDB/Twitch, Google Books et Open Library.
- La traduction facultative transmet à DeepL le texte public sélectionné à traduire, pas vos avis personnels.
- L’affichage des visuels distants, comme les images d’épisodes, certaines affiches, les fonds et les médias du magasin Steam, peut contacter leurs hébergeurs. Les nouvelles affiches principales des films et séries sont conservées localement.
- La recherche de mises à jour contacte GitHub ; elle est activée par défaut et désactivable. Le téléchargement et l’installation requièrent votre accord.
- Une bande-annonce YouTube est chargée après clic. Les services externes appliquent leurs propres règles de confidentialité, conditions et limites.
- Le lien **Soutenir NOVARIUM** ouvre Ko-fi dans votre navigateur uniquement après votre clic. Les conditions de confidentialité de Ko-fi s’appliquent sur ce site ; aucun paiement n’est traité dans NOVARIUM.
- WebView2 et Windows peuvent posséder leurs propres mécanismes de mise à jour, distincts de NOVARIUM.

Les fournisseurs et hébergeurs peuvent recevoir votre adresse IP et les informations techniques de la connexion. Les données déjà sauvegardées localement restent consultables sans Internet, sauf les images uniquement distantes.

## Import de listes publiques Trakt

Lorsque vous demandez l’aperçu d’une liste publique, NOVARIUM contacte Trakt depuis votre ordinateur pour lire son contenu. Trakt reçoit l’identifiant numérique de la liste ou, selon le lien collé, le nom public de son propriétaire et l’identifiant de la liste. La requête contient aussi l’identifiant d’application de NOVARIUM et, pour les listes paginées, le numéro et la taille de la page demandée. Trakt voit l’adresse IP de votre connexion. Vos notes, votre historique de visionnage et le contenu de votre bibliothèque locale restent privés lors de cet échange.

Si vous confirmez l’import, NOVARIUM enregistre la collection et l’ordre des œuvres dans votre profil local. TMDB ou OMDb reçoit les identifiants ou titres nécessaires pour compléter les fiches, selon la source choisie. L’import laisse la liste d’origine sur Trakt intacte.

**Comment se déconnecter de Trakt ?** L’import fonctionne sans connexion à un compte Trakt. NOVARIUM ne conserve aucun jeton personnel Trakt et ne synchronise pas la liste en arrière-plan. Pour cesser tout échange avec Trakt, il suffit de ne plus demander d’import de liste Trakt. Vous pouvez supprimer la collection et, si vous le souhaitez, les fiches importées de votre bibliothèque locale, puis vider la corbeille. Les sauvegardes existantes conservent leur copie jusqu’à leur suppression.

## Connexion à Steam

La connexion à Steam est facultative. Lorsque vous l’activez, NOVARIUM dialogue avec Steam pour authentifier le compte et synchroniser les données choisies. Les jeux, collections, favoris et, si vous l’activez, la liste de souhaits sont enregistrés dans le profil NOVARIUM. L’actualisation automatique facultative des prix consulte le magasin public avec les identifiants des jeux et DLC concernés.

Le jeton de connexion est protégé par le coffre Windows. Sur un PC compatible, vous pouvez également activer la protection TPM. Le mot de passe Steam n’est jamais enregistré. Les sauvegardes et exports ne contiennent pas le jeton. Vous pouvez gérer la connexion et les imports Steam dans **Paramètres → Importation → Jeux vidéo**.

## Clés, sauvegardes et exports

Les identifiants API sont configurés localement et ne sont pas embarqués dans les téléchargements. Les téléchargements et mises à jour publics ne demandent pas de jeton GitHub. Les paramètres API restent dans le stockage local de NOVARIUM ; n’accordez pas l’accès à vos dossiers de données à une personne non autorisée.

Les sauvegardes et exports peuvent inclure des informations personnelles. Les clés API sont exclues par défaut. Leur inclusion peut être demandée explicitement lorsque l’option est proposée. Les références des ebooks restent dans les archives créées par l’application. Conservez ces archives dans un emplacement privé.

Les sauvegardes automatiques conservent les chemins des vidéos locales et leurs associations. Pour les exports, la case **Inclure les liens des vidéos locales** est cochée par défaut pour le profil complet et décochée pour les collections. Les vidéos elles-mêmes ne sont jamais copiées dans l’archive. Si vous incluez les liens, leurs chemins peuvent révéler des noms de dossiers : vérifiez ce choix avant de partager une collection. Désactiver cette option n’anonymise pas les autres informations de l’archive, comme vos notes et les noms de collections.

Le serveur interne de l’application se limite à la boucle locale et n’est pas exposé au réseau local. La séparation des profils n’est pas une authentification destinée à protéger des données contre un autre utilisateur ayant accès au même compte Windows.

## Suppression et réinitialisation des profils

La suppression d’un profil efface définitivement les fichiers actifs identifiés comme lui appartenant, après confirmation. Les sauvegardes, les fichiers externes et les fichiers dont l’appartenance reste incertaine sont conservés. Si le dossier du profil est indisponible, le retirer du sélecteur conserve ses fichiers et ses sauvegardes. Des données de récupération et journaux techniques peuvent être conservés pour terminer une opération interrompue. La réinitialisation et la suppression sont des opérations distinctes.

La corbeille des œuvres et collections peut être vidée automatiquement après le délai choisi dans ses paramètres. Cette option est désactivée par défaut. Elle supprime les éléments concernés de la bibliothèque, sans supprimer les vidéos externes de vos dossiers.

## Signalements

Les [Issues GitHub](https://github.com/Light-x02/Novarium/issues) sont un service externe. Les messages qui y sont publiés sont visibles publiquement. Anonymisez vos captures et n’envoyez aucune clé, sauvegarde, collection complète ou fichier ebook.

## Dossiers vidéo

L’analyse des fichiers et de leur qualité s’effectue sur votre ordinateur. Les vidéos ne sont pas téléversées vers un fournisseur. Les recherches de métadonnées transmettent les titres ou identifiants nécessaires aux services sélectionnés. Les chemins des fichiers peuvent figurer dans les données du profil et ses exports : ne partagez pas ces archives publiquement. La lecture transmet le fichier à votre lecteur Windows uniquement après votre clic.
