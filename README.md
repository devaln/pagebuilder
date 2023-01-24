# Pagebuilder Installation 

Followed these steps to install Laravel Pagebuilder in this project:
- ````composer require hansschouten/laravel-pagebuilder````
- ```php artisan vendor:publish --provider="HansSchouten\LaravelPageBuilder\ServiceProvider" --tag=config```
- Updated the configuration in `config/pagebuilder.php`
- ```php artisan migrate```

Next, created a theme:
- ```php artisan pagebuilder:create-theme [theme-name]```
or only for login purpose we can publish demo theme by
- ```php artisan pagebuilder```

Then, loggedin via `/admin` with `admin` and `changethispassword` (the admin URL and credentials can be changed in the pagebuilder config file).
