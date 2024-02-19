# docker init

## これは何？

* docker init を検証するためのサンプルコード
* 生成された成果物に関する気づきについてこのファイルに簡単にまとめる

## docker init とは

* Dockerfile、compose.yamlを自動生成してくれる
* 2023.5 Docker Desktip 4.18でβ版リリース ⇒ 4.27より正式サポート開始

### Dockerfile

* alpine ベースのイメージが採用されていることが多そう
  * 使用したいイメージが他にある場合は自前で書き替えが必要
* syntax ディレクティブ
* ダウンロードした依存パッケージをキャッシュ
* 非rootユーザーで実行される

### compose.yaml

* DBはPostgreSQL固定（2024/2/19現在）

## 参考

* [docker init](https://docs.docker.com/engine/reference/commandline/init/)

* [Publickey](https://www.publickey1.jp/blog/24/dockerdocker_initdockerfilecompose.html)

* [docker blog](https://www.docker.com/blog/streamline-dockerization-with-docker-init-ga/)
