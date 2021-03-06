# **Pixels CRM API Features**

-   The Pixels CRM API is a REST API that includes the following features

    -   `User account` CRUD functionality.
    -   `Roles` CRUD functionality - `Administrator`, `Super User`, `and User`.
    -   `Customer` CRUD functionality
        -   `Customer Address` CRUD functionality.
        -   `Customer Contact` CRUD functionality.
    -   `Task` CRUD functionality: Tasks are a one-to-many polymorphic feature that can be assigned to any model except the 'User' model. This is because users can be assigned to tasks and would not make sense add tasks to the user model.
    -   `Lead` CRUD functionality
    -   `Lead Status` CRUD functionality.
    -   `Login` / `Logout` functionality.
    -   Authentication with JWT and Laravel Sanctum.
    -   Permission policies.
    -   Functional tests.

## **!! Please keep in mind this is an API only. No frontend is included !!**

&nbsp;

# **Full API Documentation**

## **Wiki**: https://pixelscrm.pixelfix.net.au

&nbsp;

# **Server Requirements**

-   PHP >= 8.0
-   BCMath PHP Extension
-   Ctype PHP Extension
-   cURL PHP Extension
-   DOM PHP Extension
-   Fileinfo PHP Extension
-   JSON PHP Extension
-   Mbstring PHP Extension
-   OpenSSL PHP Extension
-   PCRE PHP Extension
-   PDO PHP Extension
-   Tokenizer PHP Extension
-   XML PHP Extension

&nbsp;

# **Database Requirements**

-   The project is setup to use an instance of SQLite by default.
-   Any other database system compatable with Laravel can be used. Follow the recommended installation instructions for such database.

&nbsp;

# **Installation Instructions**

-   Download and unzip the project files in your desired directory.
-   Rename the `.env.example` to `.env`
-   Rename the `.env.local` to `.env.backup` or delete `.env.local`
-   Run `composer install` from within the project directory.
-   Run `php artisan key:generate` to generate a new key for your application.
-   By default the application is setup to use an SQLite database. Run `php artisan migrate` or `php artisan migrate --seed` to include seed data.
-   If you run this project locally; run `php artisan serve` and your API application will be available on `http://localhost:8000` by default.
