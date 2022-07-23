# Guide

## Docker command

### Build command
```sh
docker-compose build
```

### Start up command
```sh
docker-compose up -d
```

### Container command
```sh
docker-compose exec web bash
```

### Stop command
```sh
docker-compose down
```

### Check command
```sh
docker-compose ps
```

### Compose all delete command
```sh
docker-compose down --rmi all --volumes --remove-orphans
```

### Laravel install
```sh
composer create-project --prefer-dist laravel/laravel [project_name]
exit
docker-compose down
docker-compose.yml→./server/[Folder_name]:/var/www/html
docker-compose up -d
docker-compose exec web bash
composer install
npm i
```

### Laravel env
```env
DB_CONNECTION=mysql
DB_HOST=db
DB_PORT=3306
DB_DATABASE=laravel
DB_USERNAME=root
DB_PASSWORD=root
```

### Laravel breeze
```sh
composer require laravel/breeze --dev
php artisan breeze:install react
npm install
npm run dev
php artisan migrate
```

### Laravel logger
```sh
chown www-data storage/ -R
```

### Laravel cache clear
```sh
php artisan cache:clear
php artisan config:clear
php artisan route:clear
php artisan view:clear
```
