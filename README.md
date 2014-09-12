jenkins-base
========

Docker : CentOS6 and jenkins

## Yo

1. Dockerfileからimageの作成

		$ docker pull yukinagae/jenkins-base

2. imageからcontainerを起動
	
		$ docker run -d -p 8080:8080 yukinagae/jenkins-base

## Install Plugin (GitHubとの連携)

jenkinsのブラウザ上から下記をぽちぽちする。

`Jenkinsの管理` - `プラグインの管理` - `利用可能` - `「github plugin」(フィルター)を検索`  
- `チェックして[ダウンロードして再起動後にインストール]を押下` - `インストール完了後、ジョブがなければJenkinsを再起動する`


## Create New Job
`新規ジョブ作成` - `ジョブ名` - `フリースタイル・プロジェクトのビルド` - `OK`  
※「ソースコード管理」にGitが追加されていることを確認。

`[Git]をチェック` - `[Repository URL]に「https://github.com/yukinagae/xxx.git」を入力` - `[保存]を押下`
