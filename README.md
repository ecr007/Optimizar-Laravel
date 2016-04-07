# Optimizar Laravel
Pasos para optimizar Laravel

//Install application dependencies, such as the Laravel framework itself.

//If you run composer update in development and commit the `composer.lock`
//file to your repository, then `composer install` will install the exact
//same versions in production.

[code]composer install --no-interaction[/code]

//Clear the old boostrap/cache/compiled.php

[code]php artisan clear-compiled[/code]

//Recreate boostrap/cache/compiled.php

[code]php artisan optimize[/code]

//Migrate any database changes

[code]php artisan migrate[/code]
