
# debug-bar

https://laravel-news.com/laravel-debugbar

In your Laravel 5 project require the package:

composer require barryvdh/laravel-debugbar

Next open config/app.php and inside the ‘providers’ array add:

'Barryvdh\Debugbar\ServiceProvider',

Finally, if you wish to add the facades add this to the ‘aliases’ array:

'Debugbar' => 'Barryvdh\Debugbar\Facade',
