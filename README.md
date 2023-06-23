TP_SYMFONY
===

### Mise en place sécurité [https://symfony.com/doc/current/security.html](https://symfony.com/doc/current/security.html) :

```
composer require symfony/security-bundle
composer require symfony/maker-bundle
composer require orm
```

### Setup

- Créer base de données : `php bin/console doctrine:database:create`
- Générer les fichiers de migration basés sur les entités : `php bin/console make:migration`
- Exécuter les migrations : `php bin/console doctrine:migrations:migrate`

### Encore

`composer require symfony/webpack-encore-bundle`

### Registration

`symfony console make:auth`

### Routes

`symfony console debug:router`
