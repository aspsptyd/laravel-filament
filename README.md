## Create project laravel
```.sh
`$ composer create-project laravel/laravel laravel-filament "10.*"  or composer create-project laravel/laravel laravel-filament
```

## Setup env & create database

```.env
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=db_filament_lar10
DB_USERNAME=root
DB_PASSWORD=
```

## Running seed migrate fresh

```.sh
~$ php artisan migrate:fresh --seed
```

## Install filament admin panel

```.sh
~$ composer require filament/filament:"^3.2" -W
~$ php artisan filament:install --panels
```

![Screenshot 2024-10-08 at 01 44 26](https://github.com/user-attachments/assets/1a2ca3de-e0fe-43da-8c6e-68ae717bb4c0)

Setup connect to Repository in GitHub set no

![Screenshot 2024-10-08 at 01 44 37](https://github.com/user-attachments/assets/90a85e7c-ddd2-41e3-a57c-5410eb67c1b1)

## Run project & Access the panel

```.sh
~$ php artisan serve
```

Access URL http://127.0.0.1:8000/admin/login

![Screenshot 2024-10-08 at 01 45 57](https://github.com/user-attachments/assets/ad3c27a8-c712-41ac-9485-45e4190346b4)
