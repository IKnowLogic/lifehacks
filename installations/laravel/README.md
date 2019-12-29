*Commands for Laravel server*

Start laravel server\
`$ php artisan serve`

Start node watcher, continuous recompiling frontend code\
`$ npm run watch`

Start queue worker if server is using a queue\
`$ php artisan queue:work`

Clear cache, this sometimes fixes problems when new stuff is implemented\
`$ php artisan config:cache`