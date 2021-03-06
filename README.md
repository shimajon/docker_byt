# Best Your Title
このアプリは、求人広告のライター初心者や採用担当者が、
求人広告を書く際に「応募したい！」と思ってもらえるような
キャッチコピーを書けるよう、練習出来るサイトです。

【URL】https://www.bestyourtitle.com/

※ゲストログイン機能から気軽に、全機能をお試し頂けます※

<img src="https://user-images.githubusercontent.com/63326271/86881167-d125f600-c128-11ea-9d43-195848ed8872.gif" width="80%">


# このサイトの特徴
新規投稿の画面から、画像をクリックするだけで求人情報が自動入力されます。
この求人情報は求人広告営業を行なっていたアプリ作成者が考えた「職種別、よくあるターゲット情報」になります。
実際に様々なシチュエーションで求人キャッチコピーを考えるため有益な練習になります。

# 特に見ていただきたい点
- Dockerを使い、ECS(FARGATE)/ECRで本番環境をサーバーレスで運用している点。
- AWSを使い、ALBを通すことで常時SSL通信を行っている点。

<img src="https://user-images.githubusercontent.com/63326271/87216988-a08bc980-c37f-11ea-8c7a-46716366a1cb.jpg" width="80%">

## インフラ構成
- AWS(ECS(FARGATE)/ECR/ELB/Route53/ACM/RDS)
今回の構成でのメリットは以下の4つとなります。

## 保守性
アプリケーションはFargateで冗長化している。

## 信頼性
マネージドサービスのみを利用し、管理コストを低減している。

## セキュリティー
セキュリティーグループ設定により、不要なリクエストを受け付けないようにしている。

## 性能
FargateでAutoScaleが可能であり、リクエスト数に応じてサーバ台数を自動的に増減させることで応答性能を保つことができる。


# 機能一覧:

## ユーザー
- 認証機能
- 簡単ログイン機能
- マイページ機能
- プロフィール編集機能

## 投稿機能
- 投稿一覧
- 投稿検索
- 投稿編集
- 投稿削除
- コメント機能
- いいね機能
- ページネーション

## その他
- ページ遷移(loading)ビュー
- 新着順、ランキング順での一覧
- Google Analyticsの導入

# 使用技術一覧:
- Sass(scss)
- Hmal
- HTML/CSS
- Javascript / jQuery

## 開発環境
- Docker/docker-compose
- ruby 2.5.0
- Rails 5.2.3

## CI
- CircleCI

## テスト(実装予定)
- rubocop
- Rspec(単体、結合テスト) 

