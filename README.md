# rails_tutorial
Ruby on Rails 勉強用リポジトリ

## rails 6系 環境構築
参考
https://qiita.com/tana18/items/203122272fdb730e7383- 

- プロジェクト用ディレクトリを作成

```
mkdir プロジェクト名

# プロジェクトへ移動
cd プロジェクト名

```

- gemfileの生成

```
bundle init
```

- 作成したファイルの一番最後の行のコメントアウトを外す

```Gemfile
# frozen_string_literal: true

source "https://rubygems.org"

git_source(:github) {|repo_name| "https://github.com/#{repo_name}" }

# gem "rails"  ←この行のコメントを外す
```

- gemファイルのインストール

```
bundle install --path vendor/bundle
```

- railsプロジェクトの作成

```
bundle exec rails new .

# 最後に「.」は現在のディレクトリ示す
# 現在のディレクトリで、rails newを実施する
```

- rails サーバーを起動する

```
bundle exec rails s
```

localhost:3000で接続できる
