Mise en place sécurité :

```
composer require symfony/security-bundle
composer require symfony/maker-bundle
composer require orm
```

- Créer base de données : `php bin/console doctrine:database:create`
- Générer les fichiers de migration basés sur les entités : `php bin/console make:migration`
- Exécuter les migrations : `php bin/console doctrine:migrations:migrate`

