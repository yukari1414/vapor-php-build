### Setting up

1. Install [docker](https://hub.docker.com/editions/community/docker-ce-desktop-mac) or update it to the latest version
1. Run `composer install` on project root directory
1. Run `cp .env.example .env`
1. Fill in your AWS credentials in the `.env` file

### Uploading layer for PHP 7.3

1. Navigate to `php73`
1. Run `make distribution` (this takes a long time to compile)
1. Navigate to project root directory
1. Verify that the `$regions` array in `publish.php` file only has the region that you want to publish your layer to
1. Run `php publish.php`

### Reference

-   [Building your own layer](https://github.com/laravel/vapor-php-build/issues/3#issuecomment-541922252)
-   [Adding PHP `mongodb` extension](https://github.com/laravel/vapor-php-build/issues/3#issuecomment-596882721)
