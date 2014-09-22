jenkins-base
========

Docker : CentOS6 and jenkins

## Yo

1. Dockerfileからimageの作成

		$ docker pull yukinagae/jenkins-base

2. imageからcontainerを起動
	
		$ docker run -d -p 8080:8080 yukinagae/jenkins-base
