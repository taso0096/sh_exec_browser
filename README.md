# シェルスクリプトをPHPで実行するやつ
## 概要
ブラウザでshディレクトリ内のシェルスクリプトを取得し実行します。

## 使い方
`index.php`が置いてあるディレクトリにshディレクトリを作成し、その中にシェルスクリプトを置くだけ。  
シェルスクリプトの2行目がコメントだった場合は、ブラウザで説明として表示されます。

## 注意
- シェルスクリプト内にループがある場合はうまく表示されません。使いたい場合は結果をファイルに出力し`cat`で出力するなど工夫してください。
- POSTじゃなくてGETリクエストです。axiosでPHPにPOST投げる方法をいくつか試したんですけど出来ませんでした。
- コードが汚いです。
