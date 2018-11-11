# aws-sam-cli

`SAM Local` と呼ばれていたもの

https://aws.amazon.com/jp/about-aws/whats-new/2018/04/aws-sam-cli-releases-new-init-command/

## インストール

```sh
brew tap aws/tap
brew install aws-sam-cli
```

## sam init(nodejs)

https://docs.aws.amazon.com/ja_jp/lambda/latest/dg/serverless_app.html#serv-app-sam-init

```sh
sam init --runtime nodejs
```

## ユニットテスト

```sh
cd sam-app
cd hello_world
npm install

npm test
```

## エミュレート可能なサービスの確認

```sh
sam local generate-event --help
```

## サービス毎にエミュレート可能なイベントの確認

s3の場合

```sh
sam local generate-event s3 --help
```

### もっと詳しく

s3の場合

```sh
sam local generate-event s3 put --help
```