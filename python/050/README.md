# No.050

問題: 特定のディレクトリ内にあるテキストファイルから特定の文字列を検索して、その文字列を別の文字列で置換する自動化スクリプトを作成してください。

要件:

1. ユーザーに対象のディレクトリパス、検索する文字列、置換する文字列を入力してもらいます。
1. 指定されたディレクトリ内のすべてのテキストファイルから、検索する文字列を含む行を検索し、置換する文字列に置換します。
1. 置換された行を含むファイルを元の場所に上書き保存します。
1. プログラム実行時に、処理の成功か失敗かをログファイルに記録します。

注意:

- テキストファイルはUTF-8などのテキストエンコーディングを想定してください。
- 検索と置換は大文字と小文字を区別しないようにしてください。

指定したディレクトリ内のテキストファイルから特定の文字列を検索して、別の文字列に置換するDevOps自動化タスクを作成しています。置換の結果と処理の成功や失敗が「replace_log.txt」というログファイルに記録されます。