Docker メモ
---

## リファレンス  
### config files
* [DockerFile](https://docs.docker.com/engine/reference/builder/)
* [Docker Compose File](https://docs.docker.com/compose/compose-file/)
### commands
* [Docker commands](https://docs.docker.com/engine/reference/commandline/cli/)
* [Docker Compose commands](https://docs.docker.com/compose/reference/)

### 参考資料
理解が捗るスライド
* [コンテナ未経験新人が学ぶコンテナ技術入門(NTT徳永)](https://www.slideshare.net/KoheiTokunaga/ss-122754942)
* [Docker入門: コンテナ型仮想化技術の仕組みと使い方](https://www.slideshare.net/yuichi110/docker-introduction-42455180?qid=328d6017-cf55-4cf4-bb9d-129aa908369a&v=&b=&from_search=3)


---
## 目的別使い分け
### DockerFile
* コンテナイメージを作成する
### Docker Compose File
* コンテナの作成や起動を設定ファイルに残しておきたい
* 複数のコンテナを同時に起動したい
### Docker commands
* コンテナイメージの管理で使う
### Docker Compose commands
* Docker Compose Fileの内容でコンテナ管理に使う


---
## Dockerでできること
* ツールやサービスを環境もまるっと含めて簡単に構築/動作させる
* ホストを汚さずにツールやサービスを動作させる
* 開発環境としてコンテナを利用できる（ホストのエディタからコンテナ上でデバッグなど）


## Dockerで気をつけること
* 1コンテナでは、1ツール/サービスのみ実行する
* 永続化データはボリュームマウントする
* DockerHubの非公式ベンダー提供のイメージは必ずDockerFileを確認する
* Docker Compose コマンドで起動したらDocker Compose コマンドで終了するまでDocker Compose Fileは変更しない


以上
