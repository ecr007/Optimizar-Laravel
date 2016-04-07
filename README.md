# Optimizar Laravel
Pasos para optimizar Laravel

Install application dependencies, such as the Laravel framework itself.

If you run composer update in development and commit the `composer.lock`
file to your repository, then `composer install` will install the exact
same versions in production.

```
  composer install --no-interaction
```
Clear the old boostrap/cache/compiled.php

```
  php artisan clear-compiled
```

Recreate boostrap/cache/compiled.php

```
  php artisan optimize
```

Migrate any database changes

```
  php artisan migrate
```
