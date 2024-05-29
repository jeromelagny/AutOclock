# Guide d'Installation et de Configuration d'AutoKey

Ce guide est destiné aux utilisateurs de MacOS qui rencontrent des problèmes de caractères spéciaux (accolades, antislash, crochets, pipe et tilde) lors de l'utilisation d'une machine virtuelle Linux.

## Étape 1 : Installer AutoKey

Pour installer AutoKey, suivez ces instructions :
1. Ouvrez le terminal et entrez la commande suivante :
    ```bash
    sudo apt-get install autokey-gtk
    ```
    Cette commande va télécharger et installer AutoKey sur votre système.

## Étape 2 : Télécharger et Configurer AutOclock

1. Téléchargez le dossier AutOclock :
   - soon.

2. Insérez le dossier dans la configuration de AutoKey :
   - Dans le terminal, exécutez la commande suivante :
     ```bash
     cp -r ~/AutOclock ~/.config/autokey/data/
     ```
     Cette commande copie le dossier AutOclock dans le répertoire de configuration d'AutoKey.

## Étape 3 : Ajouter AutoKey au Démarrage de Linux

1. Ouvrez les paramètres de démarrage :
   - Cliquez sur le bouton pour afficher la liste des applications (généralement en bas à gauche de l'écran).
   - Recherchez et ouvrez l'application “Applications au démarrage”.

2. Ajoutez AutoKey au démarrage :
   - Dans la fenêtre qui s'ouvre, cliquez sur “Ajouter”.
   - Remplissez les champs comme suit :
     - **Nom** : AutOclock
     - **Commande** : autokey-gtk
   - Cliquez sur “Ajouter” pour sauvegarder.

En suivant ces étapes, AutoKey sera installé, configuré avec les bons raccourcis MacOS sur Linux, et démarrera automatiquement lors du démarrage de l'environnement.
