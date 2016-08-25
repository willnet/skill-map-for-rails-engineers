# これはなに

- Railsエンジニア向けのスキルマップです
- 要素技術の他に、これができたらお仕事で「○○できます！」と言える条件を書いています
- 絶賛書き途中です
- プルリクエストお待ちしています

# フロントエンド層

## HTML

- DOM
- セマンティックなマークアップ
- HTML5の機能＆互換性

### HTMLテンプレート言語

- いずれかのテンプレート言語を利用してHTMLを生成できる
  - erb
  - haml
  - slim
- HTMLエスケープとは何か説明できる
  - HTMLエスケープをするケースとしないケースについて説明できる
- いずれかのテンプレート言語でのHTMLエスケープのやり方がわかる

##  CSS

- CSS 記法
    - BEM
    - SMACC
    - など
- CSS 拡張言語
    - scss
    - sass
    - less
- CSS フレームワーク
    - bootstrap
    - foundation
    - など

## JavaScript

- プロトタイプ＆オブジェクト
- 無名関数
- AJAX
- ES2015
- CoffeeScript
- JavaScript フレームワーク
    - React.js
    - Vue.js
    - Angular.js
    - などなど

## フロントエンドその他    

- UI/UX
- Analytics
  - Google Analytics
  - など

# ミドルウェア層

## DB
### MySQL
### PostgreSQL

## WebServer(リバースプロキシ)
### Apache
### nginx
## AppServer
### unicorn

- unicorn の仕組みを説明できる
  - マスターを fork してワーカプロセスを作っているなど
- unicorn を本番用に設定して動かせる

### puma

- puma の仕組みを説明できる
  - スレッドを作りリクエストを処理する
  - unicorn と同じようにマルチプロセス設定もできるなど
- スレッドの仕組みとスレッドセーフについて理解している
- puma を本番用に設定して動かせる

### passenger

## nosql
### memcache
### redis
### mongodb
## Paas

- Heroku などの PaaS 環境で アプリケーションを動かすために必要な作業が説明できる
- もしくは非 PaaS 環境でアプリケーションを動かすために必要なミドルウェアや作業が説明できる

# アプリケーション層

## WWW

### HTTP

- 主要なリクエストメソッドについて説明できる
- 主要なステータスコードについて説明できる
- メディアタイプとは何か説明できる
- 主要なリクエストヘッダ、レスポンスヘッダについて説明できる
- HTTPキャッシュについて、必要なヘッダ込みで説明できる

### HTTP2

- HTTP2とは何なのか説明できる
  - HTTP1.1との比較
- HTTP2サーバを実装できる  

### SSL

- SSLとは何なのか説明できる
- SSL証明書の種類について説明できる
- Railsで、強制的にSSLを利用させるよう設定できる(HSTS)
- HSTSとは何なのか説明できる

## Ruby

- オブジェクト指向プログラミング
    - クラス＆モジュール
    - 属性＆メソッド
    - 継承＆ミックスイン
- 関数型プログラミング
    - ブロック
    - Proc＆ラムダ
- フロー制御
    - 条件分岐
    - 繰り返し
- REPL(対話型評価環境)＆デバッグ
- メタプログラミング

### rvm, rbenv

- いずれかのツールを設定して ruby のバーションの変更ができる
- プロジェクトごとにバージョンを変更する設定を書ける

### Gem

- Bundlerの役割、利点について説明できる
- Bundlerの基本的なコマンドを使える
- コンフリクトしてしまった依存関係の解決ができる
- 必要な時にGemを作ることができる

## Rails
### REST

- REST とは何か説明できる
- 特定ユーザのコメントを削除するときに必要なHTTPメソッドとパスをすぐ答えられる
- リソースとモデルを切り離して設計が出来る
- フレンドシップのリソース設計が出来る

### ルーティング
### アセットパイプライン＆プリプロセッサ

- アセットパイプラインとは何なのか説明できる
  - アセットパイプライを使わない場合と比べたメリットデメリット
- 開発環境と本番環境での設定の違いについて説明できる
- 本番時の assets ファイルをどこに配置するべきか説明できる

### MVC
### Rack

- Rack とは何なのか説明できる
- Rack middleware を書くことができる
- Rack アプリケーションを書くことができる
- 主要な Rack middleware を知っている

### spring
### UJS（jquery-ujs）
### バックグラウンドタスク
### キャッシュ

### ActiveRecord Migration

- マイグレーションファイルを作成できる
- マイグレーションを通じてインデックスを作成できる
- マイグレーションを通じて外部キーを作成できる
- マイグレーションを通じて alter table できる
- 特定のマイグレーションファイルをロールバックできる

### ActiveRecord

- 各クエリメソッドの使い方を理解している
  - where, join, limit, select, group, having など

- 各関連のメソッドの使い方とオプションを理解している
  - has_many, has_one, belongs_to
  - dependency, class_name, source, through
- eager loading の意味と、ActiveRecordでどのように実現するか説明できる
- バリデーション＆コールバック

### 認証  

- なんらかの gem を利用して、認証機能を実装できる
  - devise, sorcery など
- devise などの gem を使わずに、実装するとしたらどのように実装するか説明できる

### 認可

- なんらかの gem を利用して、認可処理を実装できる
  - CanCanCan
  - Pundit
- 認証と認可の違いについて説明できる

### I18n

### ActiveSupport

### 設定

production, development, test それぞれの環境の主な設定の違いについて説明できる

### Rake

- rake タスクを作ることができる
- rake タスクの依存関係の書き方がわかる
- rake タスクへの引数の渡し方がわかる

### ActionMailer    

### 運用

- rails、webサーバー、appサーバー、DBサーバーのログがどこに出力されるか調査出来る
- それぞれのログの各行の内容を説明できる

## SQL  

WIP

- SELECT文
    - GROUP
    - ORDER
    - LIMIT
- INSERT文＆UPDATE文
- トランザクション
- JOIN

### パフォーマンス

- スロークエリを取得し遅いクエリを特定できる
- DB のインデックスの仕組みについて説明できる(B+tree)
- explain を使ってインデックスが正しく使われているかを調査することができる
- N + 1 とは何か説明できる
- N + 1 の対策を説明できる
- N + 1 の予防策を説明できる


### API

- JSON API
- versioning
- documentation


## テスト

### 種類

- 単体テスト
- エンドツーエンドテスト

### RSpec / minitest
### capybara
### polgergeist / capybara-webkit

# インフラ層

- Iaas
    - AWS
    - さくら
    - DigitalOcean
- 仮想環境
    - Vagrant
    - Docker
    - Packer
- プロビジョニング
    - ansible
    - Chef
    - Itamae

## デプロイ

- CI
    - Jenkins
    - CircleCI
    - TravisCI
    - コードメトリクス
        - codeclimate
        - houndci
        - coverall
        - など
- 自動化
    - 継続的デプロイ
    - 継続的インテグレーション
    - サーバー監視＆ロギング
- 設定管理
- リリース管理
- セキュリティ＆データ完全性
- プラットフォーム
    - 専用環境
    - バーチャル環境
    - 抽象化された環境


- エラー監視
    - zabbix
    - nagiox
    - airbrake
- ログ
    - fluentd
    - treasure data
    - big query
- ロードバランサ
- キャッシュ
- DNS
- linux
    - プロセス
    - スレッド
    - ソケット
- テスト
  - serverspec

# 設計

- デザインパターン
- マイクロサービス設計
- API設計
- DBスキーマ設計

# 全体にまたがるもの

- Security
    - XSS
    - SQL Injection
    - など
- 情報共有
    - Slack
    - Qiita::Team
    - esa.io
    - Confluence
- Gem開発
- performance tuning
  - 計測
  - 調査
  - 改善

## Git, GitHub

- Git を仕事で利用できるのに必要なコマンドを理解している
- GitHub でプルリクエストを利用しつつ開発を進められる
- merge と rebase について説明できる

# その他

## 社内コミュニケーション
## 社外コミュニケーション
### 勉強会の参加、発表

- 月に n 回勉強会に参加し発表する

### ブログ

- 月に n 回ブログエントリを書く
- 100ブクマを超えるエントリを月に m 回書く

### OSS活動

- OSS に月に n 回 PR を出す
- GitHub の Public Activity を m 日継続する

## 見積もり
## mobile application
### iOS
### Android
## 他言語
### Go
### Erlang
### Elixir
### Haskell        

## 英語

- 基礎
	- 語彙
	- 文法
- 読む
- 書く
- 聞く
- 話す
