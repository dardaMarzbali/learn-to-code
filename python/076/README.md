# No.076

問題: ログファイルのエラー率を監視するスクリプトを作成してください。

あなたはSREエンジニアとして、アプリケーションのログファイルを監視してエラー率を定期的にチェックするスクリプトを作成する必要があります。スクリプトは、指定されたログファイル内のエラーメッセージの数をカウントし、エラー率を計算し、エラー率が一定のしきい値を超えた場合にアラートを生成する必要があります。

以下の条件に従ってプログラムを作成してください：

1. ユーザーに監視対象のログファイルのパスとエラー率のしきい値（例: 5%）を入力させます。
1. プログラムは指定されたログファイル内のエラーメッセージの数をカウントします。エラーメッセージは行ごとに含まれており、特定のパターン（例: "ERROR"）で検出されます。
1. エラー率を計算します。エラーメッセージの数をログの総行数で割り、パーセンテージとして表します。
1. 計算されたエラー率が指定されたしきい値を超えた場合、プログラムはアラートメッセージを表示します。しきい値未満の場合は通常のログメッセージを表示します。