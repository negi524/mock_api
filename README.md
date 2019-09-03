# 簡易モック API

## 利用パッケージ

1. [json-server](https://github.com/typicode/json-server)
1. [http-server](https://www.npmjs.com/package/http-server)

### json-server

#### 使い方

1. git リポジトリをクローン or ダウンロードする
1. `npm i`でパッケージをインストールする
1. レスポンスとして返却したい JSON ファイルを作成する（db.json を参考にすると良い）
1. 対象の JSON ファイルを引数にして、`npm run server`コマンドを実行する
1. `Resourses`のパスにアクセスすると、JSON が返却される

#### コマンド

db.json のデータを元に api を起動する時

```
$ npm run server db.json
```

routes のマッピングを行いたい時

```
$ npm run server db.json -- --routes routes.json
```

8080port を指定してローカルサーバを立ち上げたい時

```
$ npm run server db.json -- --port 8080
```

#### db.json の作成場所

`npm run server`の起動引数に指定できれば良いので、どこに作成しても良いです。  
git 管理外のディレクトリ`tmp`を作成してあるので、そこに格納することをお勧めします。

### http-server
