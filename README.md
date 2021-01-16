# docker-composeの立ち上げ手順
1. ターミナルで`git --version`を実行してgitがインストールされていることを確認する。
    - gitがインストールされていない場合は[1.5 使い始める - Gitのインストール](https://git-scm.com/book/ja/v2/%E4%BD%BF%E3%81%84%E5%A7%8B%E3%82%81%E3%82%8B-Git%E3%81%AE%E3%82%A4%E3%83%B3%E3%82%B9%E3%83%88%E3%83%BC%E3%83%AB)を参考にしてgitをインストールする。
    
1. ターミナルで`git clone https://github.com/daiki-fujii/video-communication-app.git`を実行してプロジェクトをローカル環境にコピーする。

1. ターミナルで`docker -v && docker-compose -v`を実行してdockerとdocker-composeがインストールされていることを確認する。
    - dockerとdocker-composeがインストールされていない場合は[DockerをMacにインストールする](https://qiita.com/kurkuru/items/127fa99ef5b2f0288b81)を参考にdockerとdocker-composeをインストールする。
    
1. ターミナルで`video-communication-app`ディレクトリへ移動し、`docker-compose build`を実行してnginxとnodeのコンテナを作成する。

1. 続けて、`docker-compose up -d`を実行してnginxとnodeのコンテナを起動する。

1. ブラウザで`localhost:8080`に接続する。(chrome推奨)
