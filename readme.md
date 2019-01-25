
# debug-bar

https://laravel-news.com/laravel-debugbar

In your Laravel 5 project require the package:

composer require barryvdh/laravel-debugbar

-------------

Next open app/provider/AppServiceProvider.php 

public function register()
    {
        if($this->app->isLocal())
        {
            $this->app->register(\Barryvdh\Debugbar\ServiceProvider::class);
        }
    }

-------------

Finally, if you wish to add the facades add this to the ‘aliases’ array:

'Debugbar' => 'Barryvdh\Debugbar\Facade',
