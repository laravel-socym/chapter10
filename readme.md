# 第二部 Chapter 10 / アプリケーション運用

## 対応表

 - [リスト10.1.4.2：Fluent\Logger\FluentLoggerクラスの登録](app/Providers/AppServiceProvider.php)
 - [リスト10.1.4.3：例外をFluentdに送信する](app/Exceptions/Handler.php)
 - [リスト10.1.5.3：カスタムヘッダを利用したエラーレスポンス実装例](app/Exceptions/Handler.php)
 - [リスト10.1.6.1：Bladeテンプレートと例外処理組み合わせパターン例](app/Exceptions/AppException.php)
 - [リスト10.1.6.2：例外処理とレスポンスを結び付ける例](app/Http/Controllers/Exception/BladeRenderAction.php)
 - [リスト10.1.6.3：JSONレスポンスと例外処理組み合わせパターン例](app/Exceptions/UserResourceException.php)
 - [リスト10.2.2.7：SlackWebhookHandlerの追加例（ Laravel 5.5以前の場合）](app/Providers/LogServiceProvider.php)
 - [リスト10.2.3.1：コンソールアプリケーションのログを分離する](app/Providers/AppServiceProvider.php)
 - [リスト10.2.3.2：アプリケーションログ分離例](app/Providers/ExtendLogServiceProvider.php)
 - [リスト10.2.4.3：Elastica\Clientクラスのインスタンス生成方法を記述](app/Providers/ElasticaServiceProvider.php)
 - [リスト10.2.6.1：createElasticaDriverメソッド実装例](app/Foundation/Logger/Writer.php)
 - [リスト10.2.6.3：LogServiceProviderクラスの拡張](app/Providers/ExtendLogServiceProvider.php)
 - [リスト10.2.6.4：アクセスログをControllerクラスからelasticsearchに送信する](app/Http/Controllers/IndexAction.php)
 
## For Docker

### setup 

```bash
$ docker-compose up -d
$ docker-compose run composer install --prefer-dist --no-interaction && composer app-setup
```

### down

```bash
$ docker-compose down
```

### コンテナのキャッシュが残っている場合

```bash
$ docker-compose build --no-cache
```
