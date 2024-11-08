# Module bundler : Demo
## Partie 1 - Initialisation du projet et de webpack

### Prérequis
- Ce dépôt Github doit être téléchargé sur votre machine. 
- `NodeJS` doit être installé, pour pouvoir initialiser un Package Node avec `Webpack`. 
- L'installeur peut être téléchargé et installé en suivant [ce lien](http://localhost/ "Site web de NodeJS").
- L'installation de NodeJS est combinée à celle du CLI `NPM`

Vous pouvez vous assurez que l'installation de `NodeJS` s'est déroulée sans problème en ouvrant un terminal / shell, et en executant la ligne de commande suivante : 

    node -v

Le résultat de cette commande devrait vous afficher un message ressemblant à celui-ci :

    v22.11.0

De la même façon, l'installation de `NPM` peut être testée avec la commande suivante : 

    npm -v

Donnant un résultat ressemblant à ceci : 
    
    10.9.0

### Initialisation du projet
Ouvrez ce projet dans Visual Studio Code, en allant dans `File`, puis en cliquant sur `Open folder...`. Vous pouvez ensuite sélectionner le dossier parent de ce projet et cliquer sur `Sélecitonner un dossier`.

Ouvrez un terminal / shell pointant sur le projet en allant dans `Terminal`, puis en cliquant sur `New terminal`. Initialisez le Projet Node avec la commande suivante : 

        npm init -y 

### Installer webpack et définir le script de build
Depuis le terminal / shell, installez les dépendances de développement `webpack` et `webpack-cli` :

        npm install -D webpack webpack-cli

Dans le fichier `package.json`, ajoutez un script qui execute la commande `webpack` : 

        {
            "name": "module-bundler-demo",
            ...
            "scripts": {
                "build": "webpack",
                "test": "echo \"Error: no test specified\" && exit 1"
            },
            ...
        }

### Lancer le script de build
Depuis le terminal, lancez la commande :

    npm run build

Un dossier `dist` a été créé avec un fichier `main.js`. Webpack est maintenant opérationnel.

### Passer à la partie 2
Pour continuer la suite de la démo, passez sur la branche `demo/partie-2`. 