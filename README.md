## 概要
laravelの開発環境用テンプレートです。

バージョン等は下記の通り
- PHP:8.1.6
- nginx:latest
- MySQL:latest
- laravel:latest

## 利用手順
1. `.env`ファイルを適当な内容に変更
2. `docker-compose up -d`でコンテナを立ち上げる
3. `docker-compose exec php-fpm sh`でコンテナに入る
4. `composer create-project --prefer-dist laravel/laravel`でプロジェクトの作成
5. `cd laravel`でプロジェクトのディレクトリに移動
6. `composer install`で必要なライブラリをインストール
7. `php artisan key:generate`でキーを作成