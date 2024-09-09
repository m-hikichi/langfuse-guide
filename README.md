# Langfuseの使い方

## Langfuseとは

Langfuseは、LLMアプリケーションの開発者がアプリケーションのパフォーマンスを向上させるためのツールです。以下の機能を提供しています。

- **トレース**<br>
    各LLMの呼び出しと関連ロジックの詳細ログを取得し、処理の流れを追跡する機能です。これにより、問題の特定やパフォーマンスの最適化が可能になります。
- **プロンプト管理**<br>
    プロンプトのバージョン管理と変更履歴の追跡を行います。これにより、プロンプトの改善やバグの修正を効率的に行うことができます。
- **応答評価**<br>
    評価指標やユーザーフィードバックを用いてモデルの応答品質を評価します。これにより、モデルのパフォーマンスを定量的に把握し、改善の方向性を見つけることができます。
- **メトリクス収集**<br>
    応答時間や使用料金等を記録し、ダッシュボードにて可視化します。これにより、リソースの使用状況を一目で確認し、コスト効率の良い運用を実現することができます。

## Get started

### Localhost (docker)
```bash
# Clone repository
git clone https://github.com/langfuse/langfuse.git
cd langfuse

# Run server and database
docker compose up -d
```

## How to use

### アカウントの作成

1. ブラウザから[http://localhost:3000](http://localhost:3000)へアクセス

2. ログイン画面が表示されるので、アカウント作成に進む
    ![](https://storage.googleapis.com/zenn-user-upload/493f9ff73ffd-20240206.png)

3. 名前、メアド、パスワードを入れてアカウント作成
    ![](https://storage.googleapis.com/zenn-user-upload/c7ecd22e3469-20240206.png)

### プロジェクトの作成＋APIキーの作成

1. ログインして、プロジェクトの作成
    ![](https://storage.googleapis.com/zenn-user-upload/a71a158ae708-20240206.png)

    ![](https://storage.googleapis.com/zenn-user-upload/091c80435801-20240206.png)

2. プロジェクトが作成され、設定画面を表示する
    ![](https://storage.googleapis.com/zenn-user-upload/da6add991a44-20240206.png)

3. 設定画面からAPIキーを作成。作成されたAPIキーを控えておく。Secret Keyはこのタイミングでしか表示されない。
    ![](https://storage.googleapis.com/zenn-user-upload/b07f22b3bcc1-20240206.png)

    ![](https://storage.googleapis.com/zenn-user-upload/078eef3df19f-20240206.png)

## LLMアプリケーションとLangfuseの連携

## パラメータや応答評価指数の追加

# 参考資料
- [Langfuseを試す](https://zenn.dev/kun432/scraps/e91c0d22ae1d99)