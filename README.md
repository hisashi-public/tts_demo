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
    - [VoiceTextAPI](https://cloud.voicetext.jp/webapi)
    - [VoiceTextAPI 無料利用登録](https://cloud.voicetext.jp/webapi/api_keys/new)
    - ./voicetext/key.txt に16バイトの鍵を格納する
- GCP Cloud TTS
    - [Google Could Platform Console](https://console.cloud.google.com/home)
    - 環境変数 GOOGLE_APPLICATION_CREDENTIALS に証明書の場所を指定する
- AWS Polly
    - [AWS Console](https://console.aws.amazon.com/?nc2=h_m_mc)
    - aws console からAWS Pollyを有効にしてもらい、アクセスキーとシークレットアクセスキーを取得する。
    - command lineから、aws configureを実行しアクセスキーとシークレットアクセスキーを設定する。



