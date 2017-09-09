# EasyLaravel
 The easiest way to setup a development environment for Laravel Framework. 

## Requirements
You need the Docker.
```
curl -sSL https://get.docker.com | sudo sh
```

## 1. Laravel command-line interface
Create your application dir. Change `~/myapp_dir/www` for your Laravel application dir.

```
mkdir -p ~/myapp_dir/www
sudo chown -R 1000.1000 ~/myapp_dir/www
```

Enter on container with Laravel CLI and create an new project.

```
docker run -v ~/myapp_dir/www:/app -p 8000:8000 --rm -it thenets/easylaravel /bin/bash
composer global require "laravel/installer"
laravel new blog
```

## 2. Start Server
```
docker run -v ~/myapp_dir/www:/app -p 8000:8000 --rm -it thenets/easylaravel php artisan serve
```
