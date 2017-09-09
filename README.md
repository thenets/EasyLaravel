# EasyLaravel
 The easiest way to setup a development environment for Laravel Framework. 

## Requirements
You need the Docker.
```
curl -sSL https://get.docker.com | sudo sh
```

## 1. Laravel command-line interface
Enter on container with Laravel CLI and create an new project.
Change `~/myapp_dir/www` for your Laravel application dir.

```
docker run -v ~/myapp_dir/www:/app -p 8000:8000 --rm -it thenets/easylaravel /bin/bash
laravel new blog
```

## 2. Start Server
```
docker run -v ~/myapp_dir/www:/app -p 8000:8000 --rm -it thenets/easylaravel php artisan serve
```
