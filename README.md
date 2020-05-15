# SYMFONY_CHAMLA


Repo PHP Symfony par Mats d'après tuto Youtube de Chamla. Installation et utilisation de Symfony 4

## Tuto 


Youtube : [SYMFONY 1/4 : 1H POUR COMPRENDRE LE FRAMEWORK !](https://www.youtube.com/watch?v=UTusmVpwJXo&t=143s)

## Installation


- Wampserver avec au moins php 7.2.3 (On ne se servira pas d'apache ou Mysql)
- Composer pour Windows
- VSCode avec "twig pack" et "emmet" pour les snippets (mais il est déjà dans le pack)

## Création du projet de base


- Création d'un projet symfony n'importe où (serveur interne) à l'aide de composer, un squelette de projet offert par symphony et le nom de notre projet.

```
composer create-project symfony/website-skeleton demo "^4.3.99"
```


Symfony a une CLI.
On utilisera le terminal dans VSCode

J'ai besoin de la libraire server, uniquement en dev (on n'en aura pas besoin en prod) :
```
cd demo;
composer require server --dev
```

## lancement du serveur sur le port 8000

```
php bin/console server:run
```


navigateur: http://localhost:8000/

## Création d'un controller

```
php bin/console make:controller
```


Il demande un nom de controller : BlogController
ça crée seul :
created: src/Controller/BlogController.php
created: templates/blog/index.html.twig

## Themes bootstrap


On va utiliser bootstrap 4, mais via [Bootswatch](https://bootswatch.com/) qui propose des thèmes utilisant bootstrap, mais avec couleurs, ombrages et styles différents.
On choisi le thème [Flatly](https://bootswatch.com/flatly/) et on va récupérer un bootstrap.min.css spécial Flatly.

## Template de base dans Symfony


Dans [\demo\template](C:\GIT\SYMFONY_CHAMLA\demo\templates) a été généré lors de la création du projet un template de base, dont la création de chaque composant peur s'inspirer.
base.html.twig
