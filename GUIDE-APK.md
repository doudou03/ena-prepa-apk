# Obtenir l'APK d'ENA Prépa (sans installer Android Studio)

Ce projet utilise Capacitor et GitHub Actions : GitHub construit l'APK gratuitement.
ATTENTION : ce dossier n'a pas pu être construit dans mon environnement (pas d'accès au SDK Android). La procédure est standard mais n'a pas été testée ici : si une erreur apparaît, envoie-moi le message du journal GitHub Actions.

## Étapes
1. Crée un dépôt GitHub (privé ou public) nommé `ena-prepa-apk`.
2. Dépose-y tout le contenu de ce dossier (y compris le dossier caché `.github`).
3. Sur GitHub : onglet **Actions** → « Construire l'APK » → **Run workflow**. Attends 5 à 10 minutes.
4. Ouvre l'exécution terminée, section **Artifacts**, télécharge `ena-prepa-apk` (un ZIP contenant `app-debug.apk`).
5. Envoie `app-debug.apk` sur ton téléphone Android. Ouvre-le et autorise « installer des applications de sources inconnues » si Android le demande.

## Mettre à jour l'application
Remplace les fichiers du dossier `www/` par la nouvelle version, puis relance l'étape 3. Tes résultats sont conservés si l'application garde le même identifiant (`sn.ena.prepa`) et que tu installes par-dessus l'ancienne version. Exporte quand même une sauvegarde JSON avant.

## Limites
- C'est un APK « debug » : parfait pour ton usage personnel, pas pour le Play Store (il faudrait un APK signé).
- L'icône est celle par défaut de Capacitor ; elle peut être remplacée plus tard.

## Plus simple, sans APK
Si tu hébergeais le dossier sur un site HTTPS (GitHub Pages), Chrome Android propose « Installer l'application » : même effet qu'une app, hors connexion.
