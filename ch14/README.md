# 14.デプロイと運用 (92日目-100日目, 2023/6/16 - 2023/6/24, 36時間)

## カリキュラム:デプロイと運用（36時間）
このカリキュラムを通して、デプロイと運用に関連するスキルを学びます。デプロイ先の選定、デプロイの設定と実行、環境変数の管理、ドメイン名の設定とSSL証明書の取得、パフォーマンスチューニングとモニタリングについて理解できるようになります。これにより、映画情報アプリケーションのデプロイと運用に関する知識が向上し、本番環境での安定した運用が可能になります。
### 1.Heroku, AWS, Vercelなどのデプロイ先選定（6時間）
- それぞれのプラットフォームの特徴と利点
- コスト、性能、利便性などの観点での比較
- プロジェクトに適したデプロイ先の選定
### 2.デプロイの設定と実行（12時間）
- 選定したプラットフォームに関するドキュメントの読解
- デプロイ用の設定ファイル（Procfile, Dockerfileなど）の作成
- デプロイコマンドの実行とデバッグ
- デプロイ後のアプリケーションの動作確認
### 3.環境変数の管理（6時間）
- 環境変数の利用目的と管理方法
- セキュアな環境変数の設定（APIキーやデータベース接続情報など）
- 開発環境と本番環境の環境変数の分離
### 4.ドメイン名の設定とSSL証明書の取得（6時間）
- ドメイン名の取得方法と設定
- DNS設定の変更
- SSL証明書の取得方法（Let's Encryptなど）
- HTTPS対応の設定
### 5.パフォーマンスチューニングとモニタリング（6時間）
- パフォーマンスチューニングの基本概念
- Webアプリケーションのパフォーマンス指標（応答時間、スループットなど）
- パフォーマンスモニタリングツールの利用（New Relic, Datadogなど）
- パフォーマンス改善の方法（キャッシング、データベース最適化など）

## 教材:Webサービスのデプロイと最終調整
- HerokuでRailsアプリケーションをデプロイ（Heroku公式ドキュメント）: https://devcenter.heroku.com/articles/getting-started-with-rails
- AWSでRailsアプリケーションをデプロイ（AWS公式ドキュメント）: https://aws.amazon.com/jp/getting-started/hands-on/deploy-ruby-on-rails/
- Railsアプリケーションのデプロイ方法比較（Qiita記事）: https://qiita.com/superizqi/items/5d5a78d6a58bc6d5c1b5
- Railsアプリケーションのパフォーマンスチューニング（Railsガイド）: https://railsguides.jp/performance_testing.html