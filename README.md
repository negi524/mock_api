# 簡易モックAPI

## 利用パッケージ

1. [json-server](https://github.com/typicode/json-server)
1. [http-server](https://www.npmjs.com/package/http-server)

### json-server

db.jsonのデータを元にapiを起動する時
```
$ npm run server db.json
```

routesのマッピングを行いたい時
```
$ npm run server db.json -- --routes routes.json
```

### http-server
