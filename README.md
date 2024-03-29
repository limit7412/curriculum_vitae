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
  - JavaScript
    - node.js
      - [電子書籍webビューアーのバックエンド開発](https://techdo.mediado.jp/entry/2019/10/29/090000)のため、Lambda@Edgeにて開発に利用
    - JQuery
      - 基幹システム開発で1年ほどの経験
    - Angular
      - SaaS開発のためで数ヶ月ほど経験。少し触れる程度。既存画面の改修や新画面のロジックなどを主に担当した
    - Vue.js
      - 趣味でのHPの作成などに利用
      - IoT案件でのコンソール開発のために利用
    - TypeScript
      - Angularと合わせて数ヶ月ほど経験
  - Bash
    - ユニケージ
      - 基幹システム開発で1年ほどの経験
  - Ruby
    - 趣味で小さなアプリを少し書いた
  - Python
    - Python3
      - ServerlessFramework（AWS Lambda）
        - SaaS開発で数ヶ月ほど経験
      - Django
        - IoT案件でのコンソール開発のために利用
  - Crystal
    - 主に個人での開発に利用
      - [HTTPサーバー](https://qiita.com/qazx7412/items/f4796bcfcb4d8400a0a3)
      - [LambdaのCustomRuntime](https://github.com/limit7412/lambda-crystal-sls)
  - Golang
    - 配信サービスのapi開発に利用
      - echo
      - gorm

### インフラ
  - AWS
    - 基幹システムのクラウド移行とリプレイス業務で利用
      - EC2
      - S3
    - SaaS開発のために利用
      - ServerlessFramework
        - Lambda
        - IAM
        - DynamoDB
        - CloudFormation
    - 電子書籍配信サービスのapi開発に利用
      - Fargate
      - CloudFront
        - Lambda@Edge
      - Aurora
        - MySQL
  - GCP
    - 過去に自分用のDockerコンテナを動かすために無料枠で利用していた

### ツール/サービス等
  - Docker
    - ローカルの開発環境のためにDockerComposeを主に利用
<!--   - Ansible
    - EC2の構築自動化のためにCloudFormationと合わせて利用していた
  - Stripe
    - SaaSの決済機能実装のために利用の検討をしていた -->

## 職務経歴

### 2022/09 - : 株式会社ambr

#### 2022/09 - : VRサービスバックエンド

### 2019/05 - 2022/08 : 株式会社メディアドゥ

#### 2019/05 - 2022/08 : 配信サービス
  - 社内外の電子書籍ストアのリクエストを受けて、エンドユーザーがコンテンツを閲覧できるurlを生成するapiサーバーとベンダーから提供を受けたビューアーを稼働させるためのapi、それらに付随するバッチの開発運用
    - インフラはFagate、Lambda@Edge
      - DBはAurora(MySQL 5.7)
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

#### 2017/05 - 2017/06 : 仮想プロジェクト
  - AWSのアカウントの情報を取得するslack bot
    - https://www.hands-lab.com/tech/entry/3061.html
    - node.js
    - AWS Lambda
