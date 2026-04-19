# オープン職務経歴書
公開用職務経歴書、転職活動というよりは自分が今まで何をしてきたかの振り返り用
[こちら](https://qiita.com/Sa2Knight/items/4af2f24fac9290d26119)や[こちら](https://qiita.com/okoysm/items/abcad0b4aefa585bc50b)を参考にさせていただいた

## 基本情報

|key|value|
|-|-|
|name|回路/kairox/qazx7412|
|birthdate|1993/12|
|Location|埼玉県 高崎線/宇都宮線沿線|
|mail|qazx7412@newgenerations.im|
|github|[limit7412](http://github.com/limit7412)|
|gitlab|[qazx7412](http://gitlab.com/qazx7412)|
|twitter|[@qazx7412](https://twitter.com/qazx7412)|
|qiita|[qazx7412](http://qiita.com/qazx7412)|
|zenn|[qazx7412](https://zenn.dev/qazx7412)|

## スキル/技術スタック

### 言語
  - Golang
    - webバックエンド開発に利用
      - echo
      - gin
      - gorm
  - JavaScript/TypeScript
    - [電子書籍webビューアーのバックエンド開発](https://techdo.mediado.jp/entry/2019/10/29/090000)（Lambda@Edge）
  - Bash
    - ユニケージ
  - Scala
    - 主にScala Cli、Scala Native、GraalVM
      - [PR未review通知](https://github.com/limit7412/no_review_notifications_slack)
      - [LambdaのCustomRuntime](https://github.com/limit7412/lambda-scala-sls)
  - Crystal
    - [GitHub通知管理](https://github.com/limit7412/github_notifications_slack)
    - [LambdaのCustomRuntime](https://github.com/limit7412/lambda-crystal-sls)
  - C#
    - E2Eテスト（DFrame）
    - VRChat向けフェイストラッキング用シェイプキー生成コンポーネント
      - [【無料】MMDのシェイプキーから顔トラ用シェイプキーを生成するやつ](https://qazx7412.booth.pm/items/7937591)

### インフラ
  - AWS
    - コンピューティング
      - EC2
        - webバックエンド、踏み台、バッチ等
      - Lambda
        - ミニバッチ、webサーバー、その他サーバーレス
      - Lambda@Edge
        - web向け電子書籍ミドルウェアのCGI移植
      - Fargate
        - webバックエンド（電子書籍配信サービス）
      - App Runner
        - webバックエンド（モバイル版Gogh）
    - データベース
      - Aurora
        - MySQL
      - DynamoDB
    - ストレージ
      - S3
    - IaC
      - ServerlessFramework
      - AWS CDK
      - CloudFormation
  - GCP
    - 過去に自分用のDockerコンテナを動かすために無料枠で利用していた
  - PlanetScale
    - RDB（モバイル版Gogh）
  - Momento
    - キャッシュ（モバイル版Gogh）
  - Cloudflare
    - 個人開発
    - 所有ドメイン管理
    - HP管理

### ツール/サービス等
  - Docker
    - ローカルの開発環境のためにDockerComposeを主に利用


## 職務経歴

### 2022/09 - : 株式会社ambr

#### 2023/10 - : Gogh（モバイル版）
  - 作業集中×アバター、ルーム作成アプリ
    - xambrからfork
    - サーバーサイドリード
  - インフラ
    - Fargate
    - AWS CDK
    - PlanetScale
      - MySQL互換
    - Momento
      - go-redisへの互換プロキシを使用
  - 言語
    - Go
      - バックエンドの他IaC（AWS CDK）でも使用
    - C#
      - E2Eテスト 

#### 2022/09 - 2023/09 : xambr
  - VRサービス用webバックエンド
    - 一定期間開催でcloseする期間限定イベントに合わせて毎回構築、削除
    - 途中からプラットフォーム化し、インフラは非開催期間でも運用しイベント以外の空間に入場可能な形に変更された
  - インフラ
    - Fargate
    - AWS CDK
      - プラットフォーム化前はCloudFormation
    - Aurora(MySQL)
    - ElastiCache for Redis 
  - 言語
    - Go
      - バックエンドの他IaC（AWS CDK）でも使用
    - C#
      - リアルタイムサーバー、E2Eテスト 

### 2019/05 - 2022/08 : 株式会社メディアドゥ

#### 2019/05 - 2022/08 : 配信サービス
  - 社内外の電子書籍ストアのリクエストを受けて、エンドユーザーがコンテンツを閲覧できるurlを生成するapiサーバーとベンダーから提供を受けたビューアーを稼働させるためのapi、それらに付随するバッチの開発運用
    - インフラ
      - Fagate
      - Lambda@Edge
      - Aurora(MySQL 5.7)
    - 言語は基本的にはGo、Lambda@EdgeのみNode.js
      - APIの開発と導入済みのwebビューアー（パッケージ製品）の調整
      - https://techdo.mediado.jp/entry/2019/10/29/090000

### 2017/04 - 2019/04 : ハンズラボ株式会社

#### 2019/01 - 2019/04 : IoT開発受託案件
  - 要件定義フェーズ終了から参加
    - IoTによるクラウド化
      - AWSとSoracom
    - 主に管理用コンソールの制作を担当
      - フロントとサーバーサイド両方を担当
        - Vue.js(vue-cli)でのSPA
        - Django（Python3.6）、Django Rest Frameworkによるサーバーサイド
        - インフラはAWSとSoracom
          - DBはAurora(MySQL 5.7)

#### 2018/10 - 2018/12 : ホームセンターMDシステム臨時テストチーム
  - 社内画像共有SaaSの開発と平行して臨時で結成されたタスクフォースチームに参加
    - 主にモンキーテストを行った

#### 2018/06 - 2018/12 : 社内画像共有SaaS開発
  - 小売や飲食の店舗と本部などの遠隔の拠点において画像を共有するサービス
    - https://post-for.com
  - ある程度できている段階からの機能や画面の追加
    - AngularとTypeScriptによるフロントエンド
    - Serverless Framework（AWS）とPythonによるサーバーサイド
  - 参加初期はフロントをその後サーバーサイドをメインに担当

#### 2017/07 - 2018/05 : ファストフードチェーンMDシステムリプレイス
  - いくつかの機能ができている段階からの参加
    - 店舗側機能のリプレイス
    - 本部側機能のクラウド移行
  - すでに完成しているアプリからforkしての実装
  - フロントとサーバーサイド両方を担当
    - JQueryによるフロントエンド
    - ユニケージ（bash）によるサーバーサイド
  - クラウド上でのインフラ構築
    - AWS
      - EC2で動くCGIとデータをバックアップするS3という構成
      - CloudFormationとAnsibleによる自動化

#### 2017/05 - 2017/06 : 研修（仮想プロジェクト）
  - AWSのアカウントの情報を取得するslack bot
    - https://www.hands-lab.com/tech/entry/3061.html
    - node.js
    - AWS Lambda
