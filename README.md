# Guide d'Installation et de Configuration d'AutoKey

Ce guide est conçu pour les utilisateurs de MacOS qui utilisent une machine virtuelle Linux et qui éprouvent des difficultés avec certains caractères spéciaux tels que les accolades, les antislash, les crochets, le pipe et le tilde.

Toutes les étapes sont à réaliser sur votre environnement Linux.

## Étape 1 : Installer et Lancer AutoKey 😏

### Pour installer et lancer AutoKey :

1. Ouvrez le terminal et entrez la commande suivante :

    ```bash
    sudo apt-get install autokey-gtk
    ```

    Cette commande va télécharger et installer AutoKey sur votre système. Lors de l'installation d'AutoKey, il est possible qu'une question vous soit posée. Répondez par "Oui" en appuyant sur la touche "O".

2. Maintenant, exécutez la commande suivante dans le terminal :

    ```bash
    autokey-gtk
    ```

    Cette commande exécute le programme Autokey en arrière-plan. Il s'agit d'une étape cruciale, car sans cela, l'étape 2.2 échouera.

    Laissez ce terminal ouvert et ouvrez un autre terminal pour continuer le guide.

## Étape 2 : Télécharger et Ajouter le dossier AutOclock 😜

### Télécharger le dossier AutOclock :

1. Dans le terminal, exécutez la commande suivante :

    ```bash
    git clone https://github.com/jeromelagny/AutOclock.git
    ```

### Insérer le dossier dans la configuration d'AutoKey :

2. Dans le terminal, exécutez la commande suivante :

    ```bash
    sudo cp -r ~/AutOclock ~/.config/autokey/data/
    ```

    Cette commande copie le dossier AutOclock dans le répertoire de configuration d'AutoKey. À la fin de la copie, il est possible qu'AutoKey affiche un message pour vous informer qu'un nouveau dossier a été ajouté à sa configuration. Il vous suffira de valider ce message.

## Étape 3 : Ajouter AutoKey au Démarrage de Linux 😎

### Ouvrez les paramètres de démarrage :

1. Cliquez sur le bouton pour afficher la liste des applications (généralement en bas à gauche de l'écran).
2. Recherchez et ouvrez l'application “Applications au démarrage”.

### Ajoutez AutoKey au démarrage :

3. Dans la fenêtre qui s'ouvre, cliquez sur “Ajouter”.
4. Remplissez les champs comme suit :
    - **Nom** : AutOclock
    - **Commande** : autokey-gtk
5. Cliquez sur “Ajouter” pour sauvegarder.
6. Redémarrez votre environnement Linux.

En suivant ces étapes, AutoKey sera installé, configuré avec les bons raccourcis MacOS sous Linux, et démarrera automatiquement lors du démarrage de l'environnement.
