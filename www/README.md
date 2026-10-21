# ENA Prépa — Cycle B, version 2.2

## Ce qui est inclus
- Programme d'entraînement sur 21 jours.
- Banque enrichie de questions psychotechniques originales : suites numériques, calcul, proportions, raisonnement verbal, logique, codage, données, etc.
- Sélection aléatoire des questions pour varier les séances et éviter de revoir systématiquement la même série.
- Correction après chaque test : réponse attendue, explication et méthode.
- Révision des erreurs, statistiques, chronomètre, thème sombre, export/import JSON.
- Fonctionnement hors ligne via PWA/service worker après le premier chargement.
- Page « Annales et épreuves » avec liens vers les ressources officielles et distinction claire entre sources officielles et simulations.

## Lancer sur ordinateur
Dans ce dossier, ouvrez un terminal et lancez `py -m http.server 8000` sous Windows (ou `python3 -m http.server 8000` sous macOS/Linux). Ouvrez `http://localhost:8000` dans un navigateur récent.

## Installer sur Android
Pour une installation PWA, hébergez le dossier sur un site HTTPS, ouvrez-le dans Chrome, chargez l’application une première fois puis choisissez « Installer l’application » ou « Ajouter à l’écran d’accueil ». Testez ensuite le mode avion.

## Important sur les annales
Les questions psychotechniques intégrées sont des exercices originaux de préparation, pas des questions officiellement distribuées par l’ENA. La page officielle décrit la nature des épreuves, mais les annales historiques ne doivent être qualifiées d'officielles qu'après vérification du document d'origine, de la session et de son contenu. Vérifiez toujours l'arrêté applicable à votre session.

## Données et sauvegarde
Les résultats restent dans le stockage local du navigateur. Exportez régulièrement la sauvegarde JSON si vous voulez la conserver ou la transférer sur un autre appareil. Cette application n'est pas affiliée à l'ENA du Sénégal.

## Historique
- v2.1 : corrections de la réponse de 2 questions (suite « 10 ; 13 ; 12 ; 15 ; 14 » et rendez-vous 17 jours après un lundi) ; correction du tableau de bord, qui affichait un mauvais numéro de jour (et lançait le mauvais test) dès le jour 2.
- Limites connues : 57 questions seulement (certains jours en contiennent moins de 15) ; jours 8 et 9 (matrices, raisonnement spatial) sans questions adaptées ; aucune annale officielle intégrée ; leçons des 21 jours non rédigées.
- v2.2 : animation de lancement ; page Annales avec l’état réel des recherches de documents (aucune annale officielle vérifiée intégrée) ; dossier de projet pour construire l’APK Android (voir ena-prepa-apk-projet.zip).
