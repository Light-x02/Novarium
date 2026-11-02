# Vos données et votre confidentialité

NOVARIUM est une application locale. Aucun compte NOVARIUM distant n’est nécessaire. Collections, profils, notes, suivis, préférences et sauvegardes sont enregistrés sur votre ordinateur. Le programme n’intègre pas de service d’analyse d’usage NOVARIUM ni d’envoi automatique de vos collections à l’éditeur.

## Connexions externes

- Les recherches et imports de métadonnées transmettent les titres, identifiants ou critères nécessaires aux fournisseurs sélectionnés : TMDB, OMDb, IGDB/Twitch, Google Books ou Open Library.
- La traduction facultative transmet à DeepL le texte public sélectionné à traduire, pas vos avis personnels.
- Certains portraits d’acteurs et affiches de filmographie sont affichés depuis des URL de fournisseurs. L’affichage peut donc entraîner une connexion à ces hébergeurs. Les portraits favoris peuvent être conservés localement.
- La recherche de mises à jour contacte GitHub ; elle est activée par défaut et désactivable. Le téléchargement et l’installation requièrent votre accord.
- Une bande-annonce YouTube est chargée après clic. Les services externes appliquent leurs propres règles de confidentialité, conditions et limites.
- WebView2 et Windows peuvent posséder leurs propres mécanismes de mise à jour, distincts de NOVARIUM.

Les fournisseurs et hébergeurs peuvent recevoir votre adresse IP et les informations techniques de la connexion. Les données déjà sauvegardées localement restent consultables sans Internet, sauf les images uniquement distantes.

## Clés, sauvegardes et exports

Les identifiants API sont configurés localement et ne sont pas embarqués dans les téléchargements. Les téléchargements et mises à jour publics ne demandent pas de jeton GitHub. Les paramètres API restent dans le stockage local de NOVARIUM ; n’accordez pas l’accès à vos dossiers de données à une personne non autorisée.

Les sauvegardes et exports de profil peuvent inclure des informations personnelles. Les clés API sont exclues par défaut, mais leur inclusion peut être demandée explicitement pour certains exports. Les fichiers ebooks ne sont copiés que si l’option complète correspondante est choisie. Conservez ces archives dans un emplacement privé.

Le serveur interne de l’application se limite à la boucle locale et n’est pas exposé au réseau local. La séparation des profils n’est pas une authentification destinée à protéger des données contre un autre utilisateur ayant accès au même compte Windows.

## Suppression et réinitialisation des profils

La suppression d’un profil secondaire retire définitivement ses données actives attestées après confirmation explicite. Elle ne supprime pas les sauvegardes conservées, anciennes quarantaines ou fichiers externes et ebooks originaux. Les journaux techniques nécessaires à la reprise d’une suppression interrompue peuvent rester dans le stockage local. Le profil principal est protégé. Les deux réinitialisations conservent un ancien état de récupération ; elles ne sont pas équivalentes à la suppression d’un profil.

## Signalements

Les [Issues GitHub](https://github.com/Light-x02/Novarium/issues) sont un service externe. Les messages qui y sont publiés sont visibles publiquement. Anonymisez vos captures et n’envoyez aucune clé, sauvegarde, collection complète ou fichier ebook.
