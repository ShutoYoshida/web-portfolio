# web-portfolio

このプロジェクトは、ポートフォリオのソースコードです。
HTML/CSS, JavaScriptの練習のため作成しました。
ポートフォリオの人物は架空の人物であり、実在しません。

## コンテナ起動

起動するときは以下のコマンドを入力します。
プロジェクトルートでコマンドを実行する必要があります。

```sh
# Start
$ docker run -dit --rm --name portfolio1 -v "$PWD/public":/usr/local/apache2/htdocs/ -p 3000:80 httpd:2.4-alpine
```

## アクセス

コンテナ起動中は、以下の URL にアクセスできます。

<http://localhost:3000/>

## コンテナ終了

制作終了時は以下のコマンドでコンテナを終了します。

```sh
$ docker stop portfolio1
```
