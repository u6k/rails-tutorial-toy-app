# Ruby on Railsチュートリアル "Toyアプリケーション" _(rails-tutorial-toy-app)_

[![Travis](https://img.shields.io/travis/u6k/rails-tutorial-toy-app.svg)](https://travis-ci.org/u6k/rails-tutorial-toy-app)
[![license](https://img.shields.io/github/license/u6k/rails-tutorial-toy-app.svg)](https://github.com/u6k/rails-tutorial-toy-app/blob/master/LICENSE)
[![GitHub tag](https://img.shields.io/github/tag/u6k/rails-tutorial-toy-app.svg)](https://github.com/u6k/rails-tutorial-toy-app/releases)
[![standard-readme compliant](https://img.shields.io/badge/readme%20style-standard-brightgreen.svg?style=flat-square)](https://github.com/RichardLitt/standard-readme)

> Ruby on Railsチュートリアル (https://railstutorial.jp/) の第2章「Toyアプリケーション」の作業を管理します。

## Install

Dockerを使用します。

```
$ docker version
Client:
 Version:       17.12.0-ce
 API version:   1.35
 Go version:    go1.9.2
 Git commit:    c97c6d6
 Built: Wed Dec 27 20:03:51 2017
 OS/Arch:       darwin/amd64

Server:
 Engine:
  Version:      17.12.0-ce
  API version:  1.35 (minimum version 1.12)
  Go version:   go1.9.2
  Git commit:   c97c6d6
  Built:        Wed Dec 27 20:12:29 2017
  OS/Arch:      linux/amd64
  Experimental: true
```

環境変数ファイルを作成します。`.env.example`を参考に、`.env`を作成します。

本番用Dockerイメージをビルドします。

```
$ docker-compose -f docker-compose.production.yml build
```

本番用Dockerコンテナを起動します。

```
$ docker-compose -f docker-compose.production.yml up -d
```

https://railstutorial.u6k.me/users/ にアクセスすると、"Hello, world!"が表示されます。

## Development

開発用Dockerイメージをビルドします。

```
$ docker-compose build
```

開発用Dockerコンテナを起動します。

```
$ docker-compose up -d
```

https://test.railstutorial.u6k.me/users/ にアクセスすると、"Hello, world!"が表示されます。

## Maintainer

- [u6k - GitHub](https://github.com/u6k/)
- [u6k.Blog()](https://blog.u6k.me/)
- [u6k_yu1 | Twitter](https://twitter.com/u6k_yu1)

## Contribute

ライセンスの範囲内で、ご自由にご使用ください。

## License

[MIT License](https://github.com/u6k/rails-tutorial-toy-app/blob/master/LICENSE)
