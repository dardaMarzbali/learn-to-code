# No.099

問題: あなたはWebサーバーのログファイルを解析する自動化スクリプトを作成する任務を受けました。ログファイルには以下のようなログエントリが含まれています。

```bash
192.168.0.1 - - [15/Aug/2023:12:45:32 +0000] "GET /page1 HTTP/1.1" 200 1234
192.168.0.2 - - [15/Aug/2023:12:47:15 +0000] "GET /page2 HTTP/1.1" 404 5678
192.168.0.3 - - [15/Aug/2023:12:48:59 +0000] "GET /page1 HTTP/1.1" 200 9876
```

各行は次の情報を含んでいます：

- IPアドレス
- リモートユーザー識別子 (通常は `-` で記述されます)
- リモートユーザー名 (通常は `-` で記述されます)
- アクセス日時
- リクエスト
- レスポンスステータス
- レスポンスサイズ

あなたのスクリプトは、ログファイルを読み込み、次の情報を取得する必要があります。

1. ユニークなIPアドレスの数。
1. 各リクエストのHTTPメソッド（"GET"、"POST"など）の分布。
1. レスポンスステータスコード（例：200、404）の分布。

この情報を取得するPythonスクリプトを作成してください。スクリプトはログファイルのパスを受け取り、上記の情報を出力する必要があります。また、スクリプトはログファイルが大きい場合にも効率的に動作するように設計する必要があります。