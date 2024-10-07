## Clone Project
```.sh
╰─○ git clone https://github.com/aspsptyd/laravel-filament.git
```

## Composer install

```.sh
╰─⠠⠵ composer install
```

## Create file .gitignore

```.gitignore
/.phpunit.cache
/node_modules
/public/build
/public/hot
/public/storage
/storage/*.key
/vendor
.env.backup
.env.production
.phpactor.json
.phpunit.result.cache
Homestead.json
Homestead.yaml
auth.json
npm-debug.log
yarn-error.log
/.fleet
/.idea
/.vscode
/.zed
```

## Checkout to branch filament/admin
```.sh
~$ git checkout filament/admin
```

## Copy file .env.example to .env And setup Database Config
```.sh
~$ cd projects/
~$ cp .env.example .env
~$ code .
```

![Screenshot 2024-10-08 at 00 46 50](https://github.com/user-attachments/assets/b1642100-182e-4eae-8763-c34ad9939a19)

```.env
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=db_filament
DB_USERNAME=root
DB_PASSWORD=
```

## Try to run And Error

![Screenshot 2024-10-08 at 00 49 15](https://github.com/user-attachments/assets/ff7f45e9-ab51-4310-bdfc-84dab122a691)

![Screenshot 2024-10-08 at 00 49 27](https://github.com/user-attachments/assets/831bf09a-e167-433a-ba86-533cea9c94c9)

to fix this issue run command 

```.sh
~$ php artisan key:generate
```

![Screenshot 2024-10-08 at 01 22 15](https://github.com/user-attachments/assets/fb2a3c64-8f5a-4fdd-ac18-f45a79da05d5)

```.sh
~$ composer update
~$ php artisan key:generate
```

run again

```.sh
~$ php artisan serve
```

![Screenshot 2024-10-08 at 01 12 40](https://github.com/user-attachments/assets/9266e442-e8ed-4fcf-a356-c5895befe7cf)

Access panel of filament URL http://127.0.0.1:8000/dashboard/login

![Screenshot 2024-10-08 at 01 24 34](https://github.com/user-attachments/assets/67c51652-ba09-4f2a-ba71-56a4be56af90)
