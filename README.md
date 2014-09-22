jenkins-base
========

Docker : CentOS6 and jenkins

## Yo

1. create image from Dockerfile

		$ docker pull yukinagae/jenkins-base

2. start container from image
	
		$ docker run -d -p 8080:8080 yukinagae/jenkins-base
