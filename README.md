# 動作環境
- OS
    - Linux / MacOS (Ubuntu 17.10 / macOS 10.13.4 で動作確認)
- パッケージ
    - sox
    - python3
    - ffmpeg
- python3 pip package
    - boto3
    - awscli
    - requests
    - google-cloud

# 鍵情報の設定方法
- voice text
    - [VoiceTextAPI 無料利用登録](https://cloud.voicetext.jp/webapi/api_keys/new) からユーザー情報を登録し、16バイトの認証情報を取得します。
    - ./voicetext/key.txt に16バイトの認証情報を格納する
- GCP Cloud TTS
    - [Google Could Platform Console](https://console.cloud.google.com/home)から、「APIとサービス」→「ライブラリ」→「Cloud Text to Speech API」を選択し、有効化します。
    - [Google Could Platform Console](https://console.cloud.google.com/home)から、「APIとサービス」→「認証情報 」を選択します
    - 「認証情報を作成」から「サービスアカウントキー」を選択し、「キーのタイプ」をJSONでキーを作成します。
    - 上記で保存されたJSONファイルの場所を環境変数 GOOGLE_APPLICATION_CREDENTIALS に指定します。
- AWS Polly
    - [AWS Console](https://console.aws.amazon.com/?nc2=h_m_mc) からAWS Pollyを有効にしてもらい、アクセスキーとシークレットアクセスキーを取得します。
    - command lineから、aws configureを実行しアクセスキーとシークレットアクセスキーを設定します。



