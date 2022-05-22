

## Description
This project demostrates a package to log your auth login events, and notify about the new devices and failed logins..

## Package
Visit https://rappasoft.com/docs/laravel-authentication-log/v1/introduction


## Running the APP
To run the project, you must have:
- **PHP** (https://www.php.net/downloads)
- **MySQL** (https://dev.mysql.com/downloads/installer)

Clone the repository to your local machine using the command
```console
$ git clone *remote repo url*
```

Create an `.env` file using the command. You can use this config or change it for your purposes.

```console
$ cp .env.example .env
```

### Environment
Configure environment variables in `.env` for dev environment based on your MYSQL database configuration and mailtrap credentials

```  
DB_CONNECTION=<YOUR_MYSQL_TYPE>
DB_HOST=<YOUR_MYSQL_HOST>
DB_PORT=<YOUR_MYSQL_PORT>
DB_DATABASE=<YOUR_DB_NAME>
DB_USERNAME=<YOUR_DB_USERNAME>
DB_PASSWORD=<YOUR_DB_PASSWORD>

MAIL_MAILER=
MAIL_HOST=
MAIL_PORT=
MAIL_USERNAME=
MAIL_PASSWORD=
MAIL_ENCRYPTION=
```

### Installation
Install the dependencies and start the server

```console
$ composer install
$ php artisan key:generate
$ php artisan migrate
$ php artisan serve
```


You should be able to visit your app at http://localhost:8000

### Testing
Register a new user and login. You will receive a new login email in your mailtrap inbox
Try to login in anothe browser then an email will be sent this new login in new device
