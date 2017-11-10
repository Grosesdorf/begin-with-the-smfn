begin-with-the-smfn
===================

Source: https://habrahabr.ru/post/301760/

clone a project

composer update

заполнить app/config/parameters.yml

$ php app/console doctrine:database:create
$ php app/console doctrine:schema:create
$ php app/console doctrine:fixtures:load

"Мы не хотим, переопределять уже существующие таблицы стилей.
Для того, чтобы функция asset правильно поключала файлы, нам нужно скопировать или связать ресурсы бандла в папке web нашего приложения. Это может быть сделано следующей командой в консоли:
php app/console assets:install web --symlink "

