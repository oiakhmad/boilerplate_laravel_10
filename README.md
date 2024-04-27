
## boiler plate laravel 10
1. clone the project when use https can use this url https://github.com/oiakhmad/boilerplate_laravel_10.git
2. run the code 'composer install' for donwload all package in use on this project
3. set up configuration 
   * create local db
   * adjust config on project laravel as 
   DB_CONNECTION=your_connection example (mysql)
   DB_HOST=your_host example (127.0.0.1)
   DB_PORT=your_port example (3306)
   DB_DATABASE=your_data_base_name
   DB_USERNAME=your_user_name
   DB_PASSWORD=your_db_password

3. migration
   - run the code 'php artisan migrate:fresh --seed for create all table on your database local'
   - factory in use for create fake data
5. for run servie can use 'php artisan serve'


## all package in use on this project
1. template admin stisla https://github.com/stisla/stisla
2. fortify https://laravel.com/docs/10.x/fortify#what-is-fortify
   
   example use 
   add page route on (app/Providers/FortifyServiceProvider.php) in fuction boot()
       Fortify::loginView(function(){
        return view('pages.auth.login');
       });

 
## feature 
5. crud users

## Noted
 -- config pagination
 'app\Providers\AppServiceProvider.php'
  add  the code  Paginator::useBootstrapFour(); on function boot()
