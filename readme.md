<img src="https://github.com/kkamara/useful/raw/main/MainClass.png" alt="MainClass.png" width=""/>

<img src="https://github.com/kkamara/useful/raw/main/movies.png" alt="movies.png" width=""/>

# laravel-10-api [![API](https://github.com/kkamara/laravel-10-api/actions/workflows/build.yml/badge.svg)](https://github.com/kkamara/laravel-10-api/actions/workflows/build.yml)

(19-Sep-2023) Laravel 10 GDPR compliant API system. I have been working with Laravel since Laravel 5.4 - www.endoflife.date/laravel

* [Using Thunder Client?](#using-thunder-client)

* [Tinker](#tinker)

* [Installation](#installation)

* [Usage](#usage)

* [Api Documentation](#api-documentation)

* [Run Tests](#run-tests)

* [Misc](#misc)

* [Contributing](#contributing)

* [License](#license)

## Using Thunder Client?

[Thunder client](https://www.thunderclient.com/) Visual Studio Code extension.

[thunder-collection_Tasks.json](https://github.com/kkamara/laravel-10-api/blob/main/database/thunder-collection_Tasks.json)

## Tinker

```bash
php artisan tinker
> $u = new \App\Models\User;
= App\Models\User {#6216}
```

## Installation

* [PHP and MySQL](https://www.apachefriends.org/download.html)
* [Yarn](https://yarnpkg.com/getting-started/install) (can be installed with `npm i -g yarn`)
* [https://laravel.com/docs/10.x/installation](https://laravel.com/docs/10.x/installation)
* [https://laravel.com/docs/10.x/mix#main-content](https://laravel.com/docs/10.x/mix#main-content)

Create our environment file.

```bash
cp .env.example .env
```

Install our app dependencies.

```bash
composer i
```

Generate app key.

```bash
# php artisan key:generate
composer run post-create-project-cmd
```

Run migrations with seeders.

```bash
php artisan migrate --seed
```

Install javascript required packages.

```bash
yarn && yarn build
# Do `yarn dev` during development to see live changes
# of your blade and js and css/scss dependencies with vite.config.js
```

## Usage

* [https://github.com/kkamara/laravel-makefile](https://github.com/kkamara/laravel-makefile)
* [https://laravel.com/docs/10.x/sail#main-content](https://laravel.com/docs/10.x/sail#main-content)

```bash
php artisan serve --port 3000
```

## Api Documentation

```bash
php artisan route:list --path=api -vvv
# example output:
...
POST       api/user ............................ login › Api\UserController@login
GET|HEAD   api/user/authorize .................. Api\UserController@authorizeUser
POST       api/user/register ................... Api\UserController@register
...
```

## Run Tests

```bash
php artisan test --testsuite=Feature
```

## Misc

[See Laravel 10 movies app.](https://github.com/kkamara/movies)

[See laravel makefile](https://github.com/kkamara/laravel-makefile)

[See Laravel 9 food nutrition facts search web app.](https://github.com/kkamara/food-nutrition-facts-search-web-app)

[See crm.](https://github.com/kkamara/crm)

[See php scraper.](https://github.com/kkamara/php-scraper)

[See amazon scraper.](https://github.com/kkamara/amazon-scraper)

[See python amazon scraper 2.](https://github.com/kkamara/selenium-py)

[See wordpress.](https://github.com/kkamara/wordpress)

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License
[BSD](https://opensource.org/licenses/BSD-3-Clause)
