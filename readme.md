# jwt-example

> A basic JWT example using Laravel and Vue.js

## Login
When you visit the page, you can login using:
```
email:    test@test.com
password: Test@123
```

## Build Setup - Backend

``` bash
# Install dependencies
composer install

# Setup your environment
cp .env.example .env
php artisan key:generate
php artisan jwt:generate

# Create and migrate the database
php artisan migrate --seed
```

## Build Setup - Frontend
``` bash
# The frontend is already compiled, but if you want to
# develop or recompile, follow those steps

# Go to the frontend directory
cd resources/frontend

# Install dependencies
npm install

# Build the single page application frontend
npm run build

# For development, change the API_LOCATION
# to your server.
# You can change the location in the config/dev.env.js file
npm run dev
```

## Using Homestead with Vagrant
``` bash
# Initialize Homestead
./vendor/bin/homestead make

# Edit Homestead.yaml and .env

# Create and migrate the database
php artisan migrate --seed

# Visit localhost:8000 or your custom url
```