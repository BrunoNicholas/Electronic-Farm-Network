# This will take you through how you wil install the app on you apache local enviroment or server.

## Installation on Linux (UNIX environment)
  1.  Make sure you have
          - at least PHP 7.x installed in your instances. 
          - Apache and MySQL-Server. (This can be easy by installing MAMP on a Mac or LAMP on Linux)
          - Composer which is a PHP package manager
  2.  Download the zipped file from this [Link](https://drive.google.com/file/d/1m3wvDE1wdhN4UeYaymqWGmG-n3DCUrpW/view?usp=sharing) and save the file to your computer.
  3.  To create an instance onto Apache, extract the file to your www root directory and make sure you give it the right permissions.
  4.  Open the e_pms directory, and edit the .env file and update it with your server credentials.
      ``` DB_CONNECTION=mysql
          DB_HOST=127.0.0.1
          DB_PORT=3306
          DB_DATABASE=e_pms
          DB_USERNAME=root
          DB_PASSWORD= ```
  5.  Now create a database called `e_pms` or whatever you would have changed it to.
  6.  Go back to the root of the project, ( `www/e_pms` ) and open a terminal or command promp from there and type in the following commands in order:
      ```composer install```
      ```composer update```
      ```php artisan migrate```
      ```php artisan db:seed```
      
  7.  Now you have the site done. go to your browser and load the instance as 
      `localhost/e_pms/public/` and either register or use the super-admin credentials as `sbnibro256@gmail.com` and paddword `dollar`.
      
      
## Installation on Windows
  1.  You can use WAMP with PHP 7.x or XAMPP with the same PHP version or higher.
  2.  Install composer to your instance and browse to your root php instance to proceed
  3.  Follow from `No. 2` of the Linux installation
  
  Done. Text me for any errors or questions with installation.
