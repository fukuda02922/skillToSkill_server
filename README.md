# skillToSkill_server

## 環境

* node:12.16.3

## プロジェクトの作成
基本的にはプロジェクト作成時のみです。
環境構築の際にはこの手順は飛ばして構わないです。

1. グローバルでインストール

`npm install -g serverless`

2. プロジェクトの作成
`serverless create --template aws-nodejs`

3. npmの初回
`npm init`

## プロジェクトの設定
ここでは、プロジェクトのチェックアウト後の設定を記載します。

1. awsを操作するツールをインストール(Mac)

`brew install awscli`

2. awsのユーザーを設定

`aws configure --profile {ユーザー名}`

* アクセスキー
* シークレットアクセスキー
* 「ap-northeast-1」を入力
* そのまま`Enter`

3. serverless.tsのプロファイル名変更

provider -> profileを変更

3. プロジェクトに必要なライブラリのインストール

`npm install`

4. デプロイしてみる

`sls deploy`