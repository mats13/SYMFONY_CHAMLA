# SYMFONY_CHAMLA
Repo PHP Symfony par Chamla. Installation et utilisation de Symfony 4

## Tuto 

Youtube : [SYMFONY 1/4 : 1H POUR COMPRENDRE LE FRAMEWORK !](https://www.youtube.com/watch?v=UTusmVpwJXo&t=143s)

## Installation
- Wampserver avec au moins php 7.2.3 (On ne se servira pas d'apache ou Mysql)
- Composer pour Windows
- VSCode avec "twig pack" et "emmet"

## Création du projet de base
- Création d'un projet symfony n'importe où (serveur interne) à l'aide de composer, un squelette de projet offert par symphony et le nom de notre projet.

```
composer create-project symfony/website-skeleton demo "^4.3.99"
```

Symfony a une CLI.
On utilisera le terminal dans VSCode

J'ai besoin de la libraire server, uniquement en dev (on n'en aura pas besoin en prod) :
```
composer require server --dev
```

