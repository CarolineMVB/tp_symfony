TP_SYMFONY
===

## Utilisation :

1. Installation
```
composer install
php bin/console doctrine:database:create
php bin/console doctrine:migrations:migrate
```

2. Utilisation

- Afficher les routes : `symfony console debug:router`
- Créer un utilisateur : visiter `/register`
- Connexion : visiter `/login`
- Admin dashboard : visiter `/admin`
- Se définir admin : dans la BDD, modifier la valeur de la colonne `roles` pour `["ROLE_ADMIN"]`

## Doc :

### Mise en place sécurité [https://symfony.com/doc/current/security.html](https://symfony.com/doc/current/security.html) :

```
composer require symfony/security-bundle
composer require symfony/maker-bundle
composer require orm
composer require friendsofsymfony/user-bundle "^3.0"
```

### Setup

- Créer base de données : `php bin/console doctrine:database:create`
- Générer les fichiers de migration basés sur les entités : `php bin/console make:migration`
- Exécuter les migrations : `php bin/console doctrine:migrations:migrate`
- Vider le cache : `bin/console cache:clear`
- Afficher les routes : `symfony console debug:router`

### Encore

`composer require symfony/webpack-encore-bundle`

### Registration

`symfony console make:auth`

### Admin

https://symfony.com/doc/6.2/the-fast-track/en/9-backend.html

```
symfony console make:admin:dashboard
```
