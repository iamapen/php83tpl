ローカルPCでphp-8.3をさっくり動かしたいときのプロジェクトテンプレ

# 使い方

1. cloneする
2. `.git` を消す
3. README、composer.json を修正する
4. 開発を始める

# コンテナの操作

## phpコンテナにシェルログイン
```bash
docker compose run --rm php bash
```

## php.ini 切り替え
`make help` でヘルプが出る

開発用php.iniに切り替え
```bash
make php-dev
```

本番用php.iniに切り替え
```bashmake
php-prod
```

## mysqlコンテナの起動
必須とは限らないので `manual` というprofileに分けている

`compose.yml` から `profiles` を外せば `docker compose up -d` で起動できる
