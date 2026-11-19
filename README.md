<p align="center"><img src="assets/novarium.svg" width="88" alt="Logo NOVARIUM"></p>

<h1 align="center">NOVARIUM</h1>
<p align="center"><strong>Explore Your Worlds</strong><br>Vos films, vos séries, vos jeux et vos lectures. Un même univers.</p>
<p align="center"><a href="https://github.com/Light-x02/Novarium/releases/latest">Télécharger la version stable</a> · <a href="INSTALLATION.md">Installer NOVARIUM</a> · <a href="ROADMAP.md">Feuille de route</a> · <a href="https://github.com/Light-x02/Novarium/issues">Signaler un problème</a> · <a href="https://ko-fi.com/light_x02">Faire un don</a></p>

---

**NOVARIUM est une application Windows gratuite et propriétaire pour organiser vos collections personnelles.** Une interface immersive, des profils indépendants et des données conservées sur votre ordinateur.

![Accueil de NOVARIUM : collections du moment, œuvre à la une et favoris](assets/novarium-home.png)

**La version actuelle est la [0.50.0](https://github.com/Light-x02/Novarium/releases/tag/v0.50.0).**

## Les nouveautés de la 0.50.0

- **Bibliothèque Steam.** Importez vos jeux, collections et favoris. Vous pouvez aussi importer votre liste de souhaits avec les prix et promotions disponibles. Le coffre Windows protège la connexion, avec une protection TPM facultative.
- **Fiches et statistiques de jeux.** Retrouvez les DLC, succès, heures de jeu et captures. Suivez vos installations Steam et consultez l’historique du temps de jeu par semaine ou par mois, à partir des synchronisations.
- **Recherche et accueil.** Enregistrez vos recherches et utilisez les filtres avancés de chaque bibliothèque. Choisissez les œuvres à la une, activez le défilement aléatoire et épinglez vos collections.
- **Films et séries.** La synchronisation complète les informations manquantes et ajoute les nouvelles saisons et les nouveaux épisodes en conservant votre suivi. Les affiches peuvent indiquer votre plateforme de streaming favorite lorsqu’elle propose l’œuvre.
- **Paramètres et sauvegardes.** Retrouvez une navigation latérale, des écrans d’import et de transfert remaniés et une analyse du stockage plus détaillée.
- **Mises à jour signées.** La 0.50.0 embarque la clé publique utilisée pour vérifier les prochaines mises à jour. Un résumé s’affiche au premier lancement après une mise à jour.

[Consulter toutes les nouveautés de cette version →](https://github.com/Light-x02/Novarium/releases/tag/v0.50.0)

## Quatre bibliothèques, toutes vos histoires

| Votre univers | Ce que vous pouvez organiser |
| --- | --- |
| **Films et séries** | Affiches, synopsis, distribution, saisons et épisodes, notes, favoris, statuts et suivi de visionnage. |
| **Jeux vidéo** | Fiches de jeux et de DLC, suivi manuel ou synchronisation Steam, installations, succès et statistiques. |
| **Romans** | Livres papier et numériques, éditions, sagas, tomes et progression de lecture. L’import de fichiers ebooks est suspendu pendant la préparation de la refonte. |
| **Collections** | Sous-collections, recherche, filtres, tri, ordre personnel et sélections mises en avant sur l’accueil. |

## Un espace qui vous ressemble

- **Accueil personnalisable** : œuvres à la une, sections réorganisables et collections du moment.
- **Métadonnées et illustrations** : recherche et prévisualisation avant import, choix d’images, recadrage et modifications personnelles.
- **Profils distincts** : collections, favoris et suivis séparés, avatar et préférences propres à chaque profil. Duplication, gestion du stockage et suppression avec confirmation.
- **Décor personnalisable** : choisissez et recadrez le fond de l’application. L’interface utilise le bleu électrique ; la personnalisation des thèmes est temporairement retirée.
- **Sauvegardes et transferts** : sauvegardes vérifiées, restauration avec confirmation, export de profils et de collections.
- **Imports** : ajout manuel, listes IMDb, dossiers vidéo et bibliothèque Steam. L’import de dossiers vidéo permet de sélectionner les fichiers en groupe, corriger les titres, choisir les correspondances et créer une collection.
- **Vidéos sur votre PC** : retrouvez vos films et séries, leur qualité vidéo et leurs informations, puis lancez leur lecture dans votre lecteur habituel. Actualisez vos dossiers et gérez les associations depuis NOVARIUM, sans déplacer les fichiers.
- **Mises à jour intégrées** : recherche au démarrage désactivable et recherche manuelle. Chaque installation demande votre accord et conserve le programme précédent.

## Sur votre ordinateur

La bibliothèque déjà enregistrée reste consultable hors ligne. Les recherches de métadonnées, certaines images distantes et la recherche de mises à jour utilisent Internet. Les données personnelles restent dans un dossier distinct du programme, par défaut `%LOCALAPPDATA%\NOVARIUM\`.

Les vidéos restent dans vos dossiers : NOVARIUM ne les déplace ni ne les supprime. Leur lecture utilise votre lecteur Windows, uniquement après votre clic. Les bandes-annonces YouTube ne sont chargées qu’après votre action.

Consulter la [confidentialité](CONFIDENTIALITE.md) et les [conditions d’utilisation](MENTIONS_LEGALES.md).

## Télécharger et démarrer

1. Télécharger **`NOVARIUM-vX.Y.Z.zip`** depuis les [versions officielles](https://github.com/Light-x02/Novarium/releases).
2. Extraire **tout** le contenu de l’archive dans un dossier accessible en écriture.
3. Ouvrir **`NOVARIUM/NOVARIUM.exe`** : NOVARIUM démarre dans sa fenêtre Windows.
4. Conserver le dossier **`_internal`** et toutes les ressources à côté de l’EXE.

**Windows 11 x64 : version testée. Windows 10 22H2 x64 : compatibilité prévue, pas encore vérifiée sur ce système.** Microsoft Edge WebView2 Runtime et .NET Framework 4.8 ou ultérieur doivent être présents. Ils sont généralement déjà installés ; les [instructions détaillées](INSTALLATION.md#composants-requis) indiquent quoi installer s’ils manquent. La version actuellement proposée est une archive complète à extraire.

[Instructions détaillées et dépannage →](INSTALLATION.md)

## Sources et crédits

Films et séries via **TMDB** et **IMDb via OMDb**, service indépendant de l’API officielle IMDb. Pour les jeux, **Steam** est la source proposée par défaut, avec **IGDB** en recherche complémentaire. Les livres utilisent **Google Books** et **Open Library**. La traduction via **DeepL** est facultative. Certains fournisseurs nécessitent vos propres identifiants API et appliquent leurs limites et conditions. Les disponibilités en France reposent sur les données TMDB/JustWatch lorsqu’elles existent.

NOVARIUM utilise l’API TMDB mais n’est ni approuvé ni certifié par TMDB. Les marques, notes, textes et illustrations de tiers restent soumis à leurs droits et conditions. Voir les [crédits et composants tiers](TIERS.md).

## Participer et obtenir de l’aide

- **Une idée ou une amélioration ?** Partagez-la dans [Idées et suggestions](https://github.com/Light-x02/Novarium/discussions/categories/id%C3%A9es-et-suggestions).
- **Une question sur l’application ?** Retrouvez la communauté dans [Questions et aide](https://github.com/Light-x02/Novarium/discussions/categories/questions-et-aide).
- **Un bug à signaler ?** [Ouvrez un signalement](https://github.com/Light-x02/Novarium/issues/new).

Pour signaler un bug, indiquez la version de NOVARIUM, la version de Windows et les étapes permettant de reproduire le problème. Joignez uniquement des captures anonymisées. **Ne publiez jamais de clé API, de jeton, de base de données, de sauvegarde ou de livre numérique.**

## Soutenir NOVARIUM

NOVARIUM est gratuit. Si vous souhaitez soutenir son développement, vous pouvez [faire un don sur Ko-fi](https://ko-fi.com/light_x02), ou cliquer sur **Soutenir NOVARIUM** en bas à droite de l’application. Ce soutien est entièrement facultatif.


---

NOVARIUM · Créé par **Light_x02** · Logiciel propriétaire gratuit. Ce dépôt héberge la présentation et les téléchargements de l’application.
